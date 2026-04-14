<div align="center">
  <h1> PROJET 7 | Résolvez les incidents de sécurité de bout en bout</h1>
  <p><b>Gérez un incident de sécurité de niveau intermédiaire (Cas complet)</b></p>

  <img src="https://img.shields.io/badge/STATUT-TERMINÉ-success?style=for-the-badge&logo=checkmarx" alt="Statut" />
  <img src="https://img.shields.io/badge/THÈME-INCIDENT_MANAGEMENT-blue?style=for-the-badge&logo=elastic" alt="Thème" />
  <img src="https://img.shields.io/badge/NIVEAU-INTERMÉDIAIRE-orange?style=for-the-badge" alt="Niveau" />
</div>

---

##  <u>OBJECTIF DU PROJET</u>

> **Pilotage de Crise et Investigation Globale**
> Ce projet consiste à piloter intégralement la réponse à un incident de cybersécurité majeur au sein d'un grand acteur de la distribution. L'objectif est de collecter de multiples alertes hétérogènes, de **séparer le "bruit" (faux positifs) de la menace réelle**, de reconstituer le scénario d'attaque complet, et de présenter des <u>plans de remédiation techniques et stratégiques</u> aux équipes métiers et sécurité.

---

##  <u>OUTILS, CONCEPTS & FRAMEWORKS</u>

La gestion de bout en bout nécessite l'orchestration parfaite de la trilogie défensive du SOC :

| Catégorie | Outils & Concepts | Application & Cas d'usage SOC |
| :--- | :--- | :--- |
| 🔍 **SIEM & EDR** | **Elasticsearch & Wazuh** | Fouille de logs centralisée (SIEM) et analyse comportementale des processus hôtes (HIDS/EDR). |
| 🎫 **SIRP** | **TheHive** | Gestion du *Case*, clustering d'alertes et qualification technique. |
| 🗺️ **Modélisation** | **MITRE ATT&CK & Clustering** | Regroupement des événements pour modéliser la *Kill Chain* de l'attaquant. |

---

##  <u>COMPÉTENCES ACQUISES & DÉPLOYÉES</u>
*(Hard & Soft Skills SOC)*

###  <u>Investigation Complexe et Corrélation (Hard Skills)</u>
* **Triage rigoureux** : Capacité à traiter 7 alertes en temps restreint en identifiant formellement les <u>faux positifs</u> (ex: scan Nmap légitime de supervision, phishing non cliqué, bruteforce échoué).
* **Reconstitution de la Kill Chain** : Modélisation de l'attaque avérée en 3 phases logiques : 
  1. *Accès initial* par bruteforce RDP sur un compte compromis depuis une IP malveillante.
  2. *Mouvement latéral et reconnaissance* via protocole SMB.
  3. *Élévation de privilèges* (création de compte) et tentative de vol d'identifiants en mémoire (<u>Dump de lsass.exe</u>).

###  <u>Élaboration de Plans d'Action (Hard Skills)</u>
* **Remédiation globale** : Conception de mesures de confinement immédiates et d'éradication à long terme pour chaque phase de l'attaque (blocage d'IP, désactivation des comptes, isolation réseau, ajout de règles SNORT et audits).

###  <u>Communication de Crise et Restitution (Soft Skills)</u>
* **Rapports exécutifs** : Capacité à consolider une investigation très technique en un <u>Rapport d'Incident actionnable</u>.
* **Présentation orale (Soutenance)** : Vulgarisation du scénario d'attaque face aux parties prenantes et <u>justification des impacts métiers</u> pour valider les décisions de sécurité.

---

## 📦 <u>LIVRABLES</u>

- [x] **Rapport d'Incident (Incident Report)** : Document exhaustif détaillant l'analyse technique, les indicateurs de compromission (IoC: IPs, comptes, EventIDs) et les plans d'action par dossier (Faux positifs vs Menaces).
- [x] **Support de Soutenance (Présentation Exécutive)** : Diaporama synthétisant le contexte, le scénario d'attaque et les recommandations stratégiques post-incident.
- [x] **Journalisation TheHive** : Captures d'écran attestant de la clôture propre et justifiée des alertes (*Close Case*) directement dans le SIRP, en conformité avec les procédures.

<br>

<div align="center">
  <a href="https://github.com/user-attachments/files/26643472/AD_P7_resolvez-les-incidents-de-securite-de-bout-en-bout_2025-09-15T053022.zip">
    <img src="https://img.shields.io/badge/TÉLÉCHARGER_L'ARCHIVE_DU_PROJET-ZIP-brightgreen?style=for-the-badge&logo=github" alt="Download" />
  </a>
</div>

---
<p align="center"><i>Réalisé dans le cadre de la certification Analyste SOC</i></p>
