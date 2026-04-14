<div align="center">
  <h1> PROJET 10 | Améliorez et automatisez la détection et le traitement des alertes</h1>
  <p><b>Ingénierie SecOps : Automatisation de la détection et réduction du MTTR</b></p>

  <img src="https://img.shields.io/badge/STATUT-TERMINÉ-success?style=for-the-badge&logo=checkmarx" alt="Statut" />
  <img src="https://img.shields.io/badge/THÈME-SECOPS_&_SOAR-blue?style=for-the-badge&logo=splunk" alt="Thème" />
  <img src="https://img.shields.io/badge/NIVEAU-EXPERT_/_SECOPS-orange?style=for-the-badge" alt="Niveau" />
</div>

---

##  <u>OBJECTIF DU PROJET</u>

> **Automatisation et Réduction du MTTR (Mean Time To Repair)**
> L'objectif de ce projet est de concevoir une architecture de sécurité automatisée pour un acteur de l'aéronautique. Face à l'explosion du volume d'alertes, l'enjeu est de **supprimer les tâches manuelles répétitives** pour permettre aux analystes de se concentrer sur l'investigation complexe. Ce projet repose sur le développement de dashboards **Splunk** avancés et de workflows **SOAR (n8n)** orchestrant des outils d'enrichissement sur-mesure (**Cortex**).

---

##  <u>ARCHITECTURE & STACK TECHNIQUE</u>

Le déploiement d'une chaîne automatisée nécessite une intégration profonde entre le SIEM, le SOAR et les API externes :

| Catégorie | Outils & Frameworks | Application & Cas d'usage SOC |
| :--- | :--- | :--- |
| 🛡️ **SIEM & Dashboarding** | **Splunk (SPL)** | Création de requêtes complexes et de vues de supervision comportementale. |
| ⚙️ **SOAR & Orchestration** | **n8n** | Automatisation du cycle de vie des alertes via Webhooks et routage intelligent. |
| 🐍 **Développement SecOps** | **Python (Cortex)** | Création d'analyseurs sur-mesure (bibliothèques `ldap3`, `requests`). |
| 📁 **SIRP** | **TheHive** | Centralisation des incidents et affichage des taxonomies d'enrichissement. |

---

##  <u>COMPÉTENCES ACQUISES & DÉPLOYÉES</u>
*(Hard & Soft Skills SOC)*

###  <u>Développement SecOps et Intégration d'API (Hard Skills)</u>
* **Développement d'Analyzers** : Capacité à coder des micro-services en Python pour connecter les outils de sécurité.
* **Cas pratique (Enrichissement Externe)** : Développement d'un analyseur d'IP interrogeant l'API `ip-api.com` pour injecter automatiquement des **Taxonomies visuelles** (Pays, FAI, VPN) dans TheHive.
* **Cas pratique (LDAP/AD)** : Développement d'un script capable d'interroger l'Active Directory via `ldap3` pour enrichir instantanément l'alerte avec le rôle et la description de la machine compromise.

###  <u>Ingénierie de Détection & Dashboarding (Hard Skills)</u>
* **Exploitation SPL Avancée** : Mise en évidence de compromissions comportementales via la donnée brute.
* **Détection "Impossible Travel"** : Conception d'un dashboard Splunk identifiant les connexions suspectes depuis plusieurs continents de manière anormale via des commandes de géolocalisation (`geostats`).

###  <u>Optimisation Opérationnelle (Soft Skills)</u>
* **Réduction drastique du MTTA/MTTR** : Le passage de l'enrichissement manuel à un workflow **100% autonome** permet de réduire le temps de réponse global.
* **Ingénierie de processus** : Capacité à repenser les flux de travail pour maximiser la valeur ajoutée des analystes L2/L3.

---

## 📦 <u>LIVRABLES</u>

- [x] **Scripts d'Analyse Python (Cortex Analyzers)** : Code source documenté (`LDAP_Machine.py` et `IP_Check.py`) incluant la gestion des requêtes et le parsing JSON.
- [x] **Captures d'Architecture (Dashboards & Workflows)** : Preuves visuelles du tableau de bord Splunk (Geomap) et des flux de données automatisés dans n8n.

<br>

<div align="center">
  <a href="https://github.com/user-attachments/files/26643529/AD_P10_ameliorez-et-automatisez-la-detection-et-le-traitement-des-alertes_2026-03-13T091601.zip">
    <img src="https://img.shields.io/badge/TÉLÉCHARGER_L'ARCHIVE_DU_PROJET-ZIP-brightgreen?style=for-the-badge&logo=github" alt="Download" />
  </a>
</div>

---
<p align="center"><i>Réalisé dans le cadre de la certification Analyste SOC</i></p>
