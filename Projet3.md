<div align="center">
  <h1> PROJET 3 | Collectez, analysez vos premiers logs et classez les alertes</h1>
  <p><b>Collectez, analysez vos premiers logs et classez les alertes</b></p>

  <img src="https://img.shields.io/badge/STATUT-TERMINÉ-success?style=for-the-badge&logo=checkmarx" alt="Statut" />
  <img src="https://img.shields.io/badge/THÈME-SIEM_&_TRIAGE-blue?style=for-the-badge&logo=elastic" alt="Thème" />
  <img src="https://img.shields.io/badge/NIVEAU-OPÉRATIONNEL-orange?style=for-the-badge" alt="Niveau" />
</div>

---

##  <u>OBJECTIF DU PROJET</u>

> **Transition Opérationnelle (Niveau N1 / Triage)**
> Ce projet marque la transition vers l'aspect opérationnel du métier d'Analyste SOC. L'objectif est de s'approprier l'environnement de travail typique d'un **MSSP** (*Managed Security Service Provider*), de manipuler de la donnée brute (Logs) et de piloter le <u>cycle de vie d'un incident</u> de bout en bout.

---

##  <u>OUTILS, CONCEPTS & FRAMEWORKS</u>

L'investigation et le triage nécessitent la maîtrise de la stack technique standard d'un centre d'opérations :

| Catégorie | Outils & Concepts | Application & Cas d'usage SOC |
| :--- | :--- | :--- |
| 📊 **SIEM** | **Elastic (ELK)** | Recherche, collecte et analyse de journaux d'événements (Logs) d'infrastructure. |
| 🎫 **SIRP** | **TheHive** | Plateforme de gestion d'incidents : création de *Cases*, import d'alertes et journalisation des tâches. |
| 📜 **Procédures** | **Playbooks & SOP** | Application de fiches réflexes pour garantir une réponse uniforme face aux menaces. |
| 🗺️ **Framework** | **MITRE ATT&CK** | Cartographie précise (ex: *Tactic Persistence TA0003*, *Technique Account Manipulation T1098*). |

---

##  <u>COMPÉTENCES ACQUISES & DÉPLOYÉES</u>
*(Hard & Soft Skills SOC)*

###  <u>Analyse Forensic et Traque dans les Logs (Hard Skills)</u>
* **Extraction d'IOCs** : Capacité à lire et extraire des <u>Indicateurs de Compromission</u> depuis des données brutes (fichiers CSV / requêtes SIEM).
* **Cas pratique d'investigation** : Identification d'une création de compte illégitime via l'analyse d'une ligne de commande malveillante (`net.exe user ... /ADD`) exécutée par un processus parent suspect (`powershell_ise.exe`).

###  <u>Triage et Qualification des Alertes (Hard Skills)</u>
* **Discrimination des événements** : Maîtrise du processus de distinction entre un Vrai Positif (*True Positive*) et un Faux Positif (*False Positive*).
* **Cas pratique de Triage** : Rejet d'une alerte "Exécution PowerShell" qualifiée en <u>Faux Positif</u> après investigation contextuelle (activité légitime d'un pentester interne), évitant ainsi l'escalade inutile au niveau N2.

###  <u>Documentation et Traçabilité (Soft Skills)</u>
* **Clôture et Justification** : Capacité à documenter et justifier méthodiquement la clôture d'une alerte (*Close Case*) dans TheHive avec des <u>preuves tangibles</u> (captures d'écran, notes d'analyse).
* **Transmission (Handover)** : Rigueur indispensable pour assurer la traçabilité en cas d'audits internes et la bonne passation entre les équipes (*Shift*).

---

## 📦 <u>LIVRABLES</u>

- [x] **Document de qualification des alertes (TheHive)** : Rapport de traitement formel couvrant 3 scénarios :
  * Création d'un compte local persistant (Analyse SIEM).
  * Exécution de script PowerShell (Qualification de Faux positif).
  * Analyse d'un E-mail Phishing (Extraction d'URLs, qualification d'urgence et impact).
- [x] **Matrice d'analyse de Logs** : Fichier de requêtage (.CSV) retraçant l'horodatage et la ligne de commande exacte utilisée lors de la compromission du serveur.

<br>

<div align="center">
  <a href="https://github.com/user-attachments/files/26643400/AD_P3_collectez-analysez-vos-premiers-logs-et-classez-les-alertes_2025-03-28T084017.zip">
    <img src="https://img.shields.io/badge/TÉLÉCHARGER_L'ARCHIVE_DU_PROJET-ZIP-brightgreen?style=for-the-badge&logo=github" alt="Download" />
  </a>
</div>

---
<p align="center"><i>Réalisé dans le cadre de la certification Analyste SOC</i></p>
