<div align="center">
<h1>PROJET 3 | Analyse de Logs et Triage d'Alertes</h1>
<p><i>Collectez, analysez vos premiers logs et classez les alertes</i></p>
</div>

OBJECTIF DU PROJET

Transition Opérationnelle (Niveau 1 / Triage) : Ce projet marque la transition vers l'aspect opérationnel et technique du métier d'Analyste SOC. L'objectif est de s'approprier l'environnement de travail typique d'un MSSP (Managed Security Service Provider), de manipuler la donnée brute (Logs) au sein d'un SIEM, et de piloter le cycle de vie d'un incident de bout en bout via un SIRP (Security Incident Response Platform).

OUTILS, CONCEPTS & FRAMEWORKS UTILISÉS

Outils d'investigation SOC

Elastic (SIEM) : Utilisation de la pile ELK pour la recherche, la collecte et l'analyse de journaux d'événements (Logs) d'infrastructure.

TheHive (SIRP) : Utilisation de la plateforme de référence pour la gestion de crise, l'importation d'alertes, la création de Cases (tickets d'incidents) et la journalisation des tâches (Tasks Logs).

Concepts d'analyse

Fiches réflexes (Playbooks) : Application de procédures standardisées (SOP - Standard Operating Procedures) pour garantir une réponse uniforme face aux menaces.

MITRE ATT&CK : Cartographie précise des menaces analysées (ex: Tactic Persistence TA0003, Technique Account Manipulation T1098).

COMPÉTENCES ACQUISES & DÉPLOYÉES

(Hard & Soft Skills SOC)

Analyse Forensic et Traque dans les Logs (Hard Skills)

Extraction d'IOCs : Capacité à lire et extraire des Indicateurs de Compromission depuis des données brutes (fichiers CSV / requêtes SIEM).

Cas pratique réalisé : Identification d'une création de compte illégitime (FORMASUP) via l'analyse d'une ligne de commande malveillante (net.exe user ... /ADD) exécutée par un processus parent suspect (powershell_ise.exe) sur le serveur SRV-FORMASUP-001.

Triage et Qualification des Alertes (Hard Skills)

Discrimination des événements : Maîtrise du processus de discrimination entre un Vrai Positif (True Positive) et un Faux Positif (False Positive).

Cas pratique réalisé : Rejet d'une alerte "Exécution PowerShell" qualifiée en Faux Positif après investigation contextuelle (activité légitime du service IT Sécurité / pentester), évitant ainsi l'escalade inutile.

Documentation et Traçabilité (Soft Skills & Rigueur)

Clôture et Justification : Capacité à documenter et justifier méthodiquement la clôture d'une alerte (Close Case) dans TheHive avec des preuves tangibles (captures d'écran, notes d'analyse).

Transmission : Rigueur indispensable pour les audits internes et la passation (Handover) entre les équipes (Shift).

LIVRABLES

[x] Document de qualification des alertes (TheHive) : Rapport de traitement formel couvrant 3 scénarios d'investigation distincts :

Création d'un compte local persistant (Analyse SIEM).

Exécution de script PowerShell (Qualification de Faux positif).

Analyse d'un E-mail suspect / Phishing (Extraction de liens, qualification d'urgence et évaluation de l'impact).

[x] Matrice d'analyse de Logs : Fichier de requêtage (.CSV) retraçant l'horodatage et la ligne de commande exacte utilisée lors de l'incident de compromission du serveur.

[AD_P3_collectez-analysez-vos-premiers-logs-et-classez-les-alertes_2025-03-28T084017.zip](https://github.com/user-attachments/files/26643400/AD_P3_collectez-analysez-vos-premiers-logs-et-classez-les-alertes_2025-03-28T084017.zip)
