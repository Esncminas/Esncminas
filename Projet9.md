<div align="center">
  <h1> PROJET 8 | Limitez les faux positifs</h1>
  <p><b>Optimisez en continu le système de détection et de gestion des connaissances</b></p>

  <img src="https://img.shields.io/badge/STATUT-TERMINÉ-success?style=for-the-badge&logo=checkmarx" alt="Statut" />
  <img src="https://img.shields.io/badge/THÈME-DETECTION_ENGINEERING-blue?style=for-the-badge&logo=elastic" alt="Thème" />
  <img src="https://img.shields.io/badge/NIVEAU-AVANCÉ-orange?style=for-the-badge" alt="Niveau" />
</div>

---

##  <u>OBJECTIF DU PROJET</u>

> **Amélioration Continue et Tuning**
> L'objectif de ce projet est d'adopter une posture d'amélioration continue face au risque d'<u>Alert Fatigue</u>. Il s'agit d'optimiser les règles de détection (*Tuning*) pour **réduire drastiquement les Faux Positifs**, et de capitaliser sur les retours d'expérience (*Lessons Learned*) pour enrichir la base de connaissances interne (*Knowledge Management*) via l'élaboration de <u>Playbooks</u>.

---

##  <u>OUTILS, CONCEPTS & FRAMEWORKS</u>

La réduction du bruit nécessite la maîtrise des langages de détection agnostiques et des processus de capitalisation :

| Catégorie | Outils & Concepts | Application & Cas d'usage SOC |
| :--- | :--- | :--- |
| 🛡️ **Detection Rules** | **Format Sigma (YAML)** | Écriture et optimisation de règles de détection génériques, transposables sur n'importe quel SIEM. |
| 📊 **SIEM** | **Elasticsearch** | Création de règles natives et gestion des listes d'exceptions (*Whitelists / Exception Lists*). |
| 📚 **Capitalisation** | **Playbooks & Rule Lifecycle** | Élaboration de fiches réflexes (SOPs) et audit du cycle de vie des règles de sécurité. |

---

##  <u>COMPÉTENCES ACQUISES & DÉPLOYÉES</u>
*(Hard & Soft Skills SOC)*

###  <u>Tuning et Réduction des Faux Positifs (Hard Skills)</u>
* **Affinage de règles** : Capacité à rendre une règle "silencieuse" sur les comportements légitimes tout en restant intraitable sur les menaces réelles.
* **Cas pratique (Sigma)** : Optimisation d'une règle détectant les attaques Brute-Force (<u>EventID 4625</u>) par l'ajout de filtres d'exclusion ignorant les comptes de service connus (`svc_test`) et les comptes déjà verrouillés.
* **Cas pratique (Elastic)** : Création d'une règle "Scan de ports" incluant une liste d'exceptions (*Whitelist*) pour autoriser l'adresse IP du scanner de vulnérabilités interne (`192.168.9.10`), évitant le déclenchement intempestif d'alertes.

###  <u>Évaluation Stratégique de la Détection (Hard Skills)</u>
* **Audit de pertinence** : Capacité à évaluer et justifier le rejet de règles inadaptées au périmètre d'un SOC.
* **Cas pratique** : Rejet justifié d'une règle d'alerte sur un "Espace disque à 70%", requalifiée en incident de supervision système (<u>Monitoring IT</u>) et non en incident Cyber.
* 
###  <u>Capitalisation et Vulgarisation (Soft Skills)</u>
* **Structuration de l'information** : Capacité à structurer la connaissance pour faciliter l'intégration (*Onboarding*) et les passations d'équipe (*Handover*).
* **Création de Playbooks** : Amélioration technique d'une fiche d'investigation Wazuh (analyse d'élévation de privilèges via les champs `TokenElevationType`) et création intégrale d'un <u>Playbook de qualification de Phishing</u>.

---

## 📦 <u>LIVRABLES</u>

- [x] **Rapport d'optimisation de la détection** : Document d'expertise justifiant la sélection ou le rejet technique de 5 règles de détection proposées.
- [x] **Règles de Détection Optimisées (Code)** : Fichier générique (`.yaml`) codé au standard Sigma ciblant les échecs d'authentification, et export de règle SIEM Elastic (`.ndjson`) incluant la gestion d'une liste d'exceptions.
- [x] **Base de Connaissances / Playbooks** : Livrables opérationnels comprenant une fiche réflexe entièrement créée (Traitement de Phishing) et une fiche améliorée techniquement (Investigation Wazuh).

<br>

<div align="center">
  <a href="https://github.com/user-attachments/files/26643480/AD_P8_limitez-les-faux-positifs_2025-10-23T130258.zip">
    <img src="https://img.shields.io/badge/TÉLÉCHARGER_L'ARCHIVE_DU_PROJET-ZIP-brightgreen?style=for-the-badge&logo=github" alt="Download" />
  </a>
</div>

---
<p align="center"><i>Réalisé dans le cadre de la certification Analyste SOC</i></p>
