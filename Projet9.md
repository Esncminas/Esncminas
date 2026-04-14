<div align="center">
  <h1> PROJET 9 | Appuierez-vous sur le bouton rouge ?</h1>
  <p><b>Résolvez un incident de sécurité complexe (Gestion de Crise / CSIRT)</b></p>

  <img src="https://img.shields.io/badge/STATUT-TERMINÉ-success?style=for-the-badge&logo=checkmarx" alt="Statut" />
  <img src="https://img.shields.io/badge/THÈME-CSIRT_&_CRISIS-blue?style=for-the-badge&logo=windows" alt="Thème" />
  <img src="https://img.shields.io/badge/NIVEAU-EXPERT-red?style=for-the-badge" alt="Niveau" />
</div>

---

##  <u>OBJECTIF DU PROJET</u>

> **Gestion de Crise (CSIRT)**
> Ce projet est une simulation de gestion de crise cyber majeure (Niveau CSIRT - *Computer Security Incident Response Team*). L'objectif est d'intervenir en urgence pour une grande entreprise du secteur de l'énergie subissant une **attaque APT fulgurante** ayant conduit à la compromission de son **Contrôleur de Domaine (Active Directory)**. Il s'agit d'analyser l'intrusion, de stopper l'exfiltration de données critiques, de nettoyer l'infrastructure et de rassurer les instances dirigeantes via une communication de crise maîtrisée.

---

##  <u>OUTILS, CONCEPTS & FRAMEWORKS</u>

La gestion de crise de niveau CSIRT nécessite de comprendre l'attaque à très bas niveau pour appliquer une défense chirurgicale :

| Catégorie | Outils & Concepts | Application & Cas d'usage SOC |
| :--- | :--- | :--- |
| 🏴‍☠️ **Offensif (APT)** | **MITRE ATT&CK & AD** | *Spear Phishing*, *Typosquatting*, *HTML Smuggling* et backdoors Active Directory. |
| 📡 **Exfiltration** | **DNS Tunneling** | Détection et analyse de fuites de données encodées via des requêtes DNS over TCP (port 53). |
| 🛡️ **Défense Réseau** | **Snort (IDS/IPS)** | Création de règles de blocage réseau ciblées pour endiguer immédiatement la compromission. |

---

##  <u>COMPÉTENCES ACQUISES & DÉPLOYÉES</u>
*(Hard & Soft Skills SOC)*

###  <u>Forensic et Rétro-ingénierie d'Exfiltration (Hard Skills)</u>
* **Analyse de flux furtif** : Capacité à décortiquer une technique de vol de données silencieuse (*Data Leak*).
* **Cas pratique (Décodage)** : Identification d'un flux DNS suspect. Extraction des sous-domaines, puis <u>conversion du payload depuis le format Hexadécimal vers l'ASCII</u> pour prouver la nature de la fuite : un dump complet des comptes Active Directory et des mots de passe administrateurs en clair.

###  <u>Endiguement et Éradication Systémique (Hard Skills)</u>
* **Disaster Recovery** : Capacité à formuler et appliquer un plan de reprise d'activité immédiat.
* **Cas pratique Réseau (Snort)** : Écriture d'une règle personnalisée (`block tcp $HOME_NET 53 -> 183.251.167.28 53`) pour **couper net le tunnel d'exfiltration**.
* **Cas pratique Système (AD)** : Planification du nettoyage chirurgical de l'Active Directory (suppression des comptes pirates, destruction des tâches planifiées, nettoyage du registre) couplée à un *"Force Reset"* massif des comptes compromis.

###  <u>Gestion de Crise et Restitution Executive (Soft Skills)</u>
* **Traduction stratégique (C-Level)** : Capacité à traduire l'urgence technique en langage stratégique pour les niveaux de direction.
* **Vulgarisation de crise** : Utilisation de l'analogie (ex: expliquer le *Tunneling DNS* aux équipes métiers en le comparant à un découpage de données envoyé en "code morse") pour <u>justifier et faire accepter les coupures de services urgentes</u>.

---

## 📦 <u>LIVRABLES</u>

- [x] **Rapports d'Investigation et de Remédiation** : Exports détaillés du SIRP (TheHive / PDF) attestant de l'identification de la Kill Chain complète et de la liste exacte des actions curatives (Équipes Système, Réseau et AD).
- [x] **Support de Présentation de Crise (PPTX)** : Diaporama exécutif à destination de la direction de l'entreprise (Résumé de la situation, chronologie technique, impacts et mesures de remédiation).
- [x] **Règle de Détection/Blocage (Code)** : Fichier contenant la règle Snort opérationnelle pour neutraliser la fuite de données (Drop du flux TCP/53).

<br>

<div align="center">
  <a href="https://github.com/user-attachments/files/26643519/AD_P9_appuierez-vous-sur-le-bouton-rouge_2026-01-19T084129.zip">
    <img src="https://img.shields.io/badge/TÉLÉCHARGER_L'ARCHIVE_DU_PROJET-ZIP-brightgreen?style=for-the-badge&logo=github" alt="Download" />
  </a>
</div>

---
<p align="center"><i>Réalisé dans le cadre de la certification Analyste SOC</i></p>
