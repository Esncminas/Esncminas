<div align="center">
<h1>PROJET 7 | Gestion d'Incident et Corrélation</h1>
<p><i>Gérez un incident de sécurité de niveau intermédiaire</i></p>
</div>

OBJECTIF DU PROJET

Pilotage de Crise et Investigation : Ce projet consiste à piloter intégralement la réponse à un incident de cybersécurité majeur au sein d'un grand acteur de la distribution (Carochan). L'objectif est de collecter de multiples alertes hétérogènes, de séparer le "bruit" (faux positifs) de la menace réelle, de reconstituer le scénario d'attaque complet, et de présenter des plans de remédiation techniques et stratégiques aux équipes métiers et sécurité.

OUTILS, CONCEPTS & FRAMEWORKS UTILISÉS

Outils SOC

Plateformes SOC  : Utilisation conjointe d'Elasticsearch (SIEM pour la fouille de logs), Wazuh (EDR/HIDS pour l'analyse des processus hôtes) et TheHive (SIRP pour la gestion du Case et la qualification).

Concepts d'Analyse

Framework MITRE ATT&CK : Cartographie de la progression de l'attaquant (Accès Initial, Reconnaissance, Maintien dans les lieux, Vol d'identifiants).

Méthodologie d'Investigation : Regroupement par "Dossiers" (Clustering d'alertes) pour identifier les liens temporels et logiques entre différents événements isolés.

COMPÉTENCES ACQUISES & DÉPLOYÉES

(Hard & Soft Skills SOC)

Investigation Complexe et Corrélation (Hard Skills)

Traitement d'alertes : Capacité à traiter et catégoriser 7 alertes distinctes en un temps restreint.

Triage rigoureux : Identification formelle de faux positifs (ex: scan Nmap légitime de supervision, phishing non cliqué, bruteforce échoué sur printer3).

Reconstitution de la Kill Chain : Modélisation de l'attaque avérée en 3 phases logiques : 1) Accès initial par bruteforce RDP sur le compte carter depuis l'IP malveillante kali, 2) Mouvement latéral et reconnaissance via protocole SMB, 3) Élévation de privilèges (création du compte ext-adm) et tentative de vol de mots de passe en mémoire (Dump de lsass.exe).

Élaboration de Plans d'Action (Hard Skills)

Remédiation globale : Conception de mesures de remédiation immédiates (Containment) et à long terme (Eradication/Recovery) pour chaque phase de l'attaque : blocage d'IP externe, désactivation des comptes compromis, isolation réseau, ajout de règles de détection SNORT et audits SMB.

Communication de Crise et Restitution (Soft Skills)

Rapports exécutifs : Capacité à consolider une investigation très technique en un Rapport d'Incident clair, structuré et actionnable.

Présentation orale (Soutenance) : Vulgarisation du scénario d'attaque face aux parties prenantes et justification des impacts métiers pour valider les décisions de sécurité.

LIVRABLES

[x] Rapport d'Incident (Incident Report) : Document exhaustif détaillant l'analyse technique des alertes, les indicateurs de compromission (IoC: IPs, comptes, EventIDs) et les plans d'action par dossier (Faux positifs vs Menaces).

[x] Support de Soutenance (Présentation Exécutive) : Diaporama synthétisant le contexte, la méthodologie, le scénario d'attaque reconstitué et les recommandations stratégiques post-incident.

[x] Journalisation TheHive : Captures d'écran attestant de la clôture propre et justifiée des alertes (Close Case) directement dans le SIRP, en conformité avec les procédures d'un SOC professionnel.

[AD_P7_resolvez-les-incidents-de-securite-de-bout-en-bout_2025-09-15T053022.zip](https://github.com/user-attachments/files/26643472/AD_P7_resolvez-les-incidents-de-securite-de-bout-en-bout_2025-09-15T053022.zip)
