<div align="center">
  <h1> PROJET 4 | Rédigez vos premiers scripts en Python </h1>
  <p><b>Rédigez vos premiers scripts en Python d'automatisation SOC</b></p>

  <img src="https://img.shields.io/badge/STATUT-TERMINÉ-success?style=for-the-badge&logo=checkmarx" alt="Statut" />
  <img src="https://img.shields.io/badge/THÈME-AUTOMATISATION_&_PYTHON-blue?style=for-the-badge&logo=python" alt="Thème" />
  <img src="https://img.shields.io/badge/NIVEAU-SCRIPTING-orange?style=for-the-badge" alt="Niveau" />
</div>

---

##  <u>OBJECTIF DU PROJET</u>

> **Automatisation de la Réponse (Incident Response)**
> Ce projet introduit la programmation comme levier fondamental pour l'automatisation de la réponse aux incidents. L'objectif est de concevoir un outil en Python capable d'analyser une arborescence de serveurs web clients, de détecter des <u>Web Shells</u> ou scripts malveillants basés sur des indicateurs de compromission (IoC), et d'appliquer une <u>mesure de remédiation automatisée</u> (Neutralisation).

---

##  <u>OUTILS, CONCEPTS & FRAMEWORKS</u>

La création d'outils de sécurité internes nécessite une bonne compréhension du système de fichiers et des principes de préservation :

| Catégorie | Outils & Concepts | Application & Cas d'usage SOC |
| :--- | :--- | :--- |
| 💻 **Langage & Env.** | **Python 3 (`os`)** | Utilisation de la bibliothèque standard pour les interactions profondes avec le système de fichiers. |
| 🔍 **Détection** | **IoC Matching** | Recherche d'Indicateurs statiques (noms de fichiers) et dynamiques (IP de Command & Control cachée). |
| 🛡️ **Remédiation** | **Defanging** | Technique de *neutralisation* consistant à rendre une menace inopérante sans détruire l'artefact. |

---

##  <u>COMPÉTENCES ACQUISES & DÉPLOYÉES</u>
*(Hard & Soft Skills SOC)*

###  <u>Développement d'Outils de Sécurité (Hard Skills)</u>
* **Création de script d'investigation** : Développement itératif d'outils d'analyse (Scripts 1 à 4).
* **Analyse de fichiers** : Capacité à parcourir récursivement des répertoires (`os.walk`), lire et décortiquer le contenu des fichiers pour y traquer une <u>adresse IP malveillante</u> (`8.13.193.9`) ou identifier un préfixe suspect (`xmc6_`).

###  <u>Remédiation et Préservation des Preuves (Hard Skills)</u>
* **Gestion d'incident (NIST)** : Maîtrise des concepts de réponse à incident en phase de Confinement et d'Éradication (*Containment & Eradication*).
* **Cas pratique de Defanging** : Prise de décision technique cruciale via le <u>renommage des fichiers infectés</u> (ajout de l'extension `.txt`) plutôt que leur suppression. Cela casse l'exécution côté serveur (ex: neutralisation d'un `.php`) tout en <u>préservant le code source intact</u> pour l'équipe d'investigation numérique (Forensic / Reverse Engineering).

###  <u>Logique Algorithmique (Soft Skills)</u>
* **Décomposition de problèmes** : Capacité à scinder un problème d'investigation complexe en sous-tâches simples (Lister les fichiers ➡️ Trouver les cibles ➡️ Lire le contenu ➡️ Appliquer la neutralisation).

---

## 📦 <u>LIVRABLES</u>

- [x] **Code Source (Python)** : Script complet (`Script 4.py`) intégrant la gestion des erreurs
