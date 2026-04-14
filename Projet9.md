<div align="center">
<h1>PROJET 9 |Appuierez-vous sur le bouton rouge ?Complexe</h1>
<p><i>Résolvez un incident de sécurité complexe (Gestion de Crise)</i></p>
</div>

OBJECTIF DU PROJET

Gestion de Crise (CSIRT) : Ce projet est une simulation de gestion de crise cyber majeure (Niveau CSIRT - Computer Security Incident Response Team). L'objectif est d'intervenir en urgence pour une grande entreprise du secteur de l'énergie (Echelon) subissant une attaque fulgurante ayant conduit à la compromission de son Contrôleur de Domaine (Active Directory). Il s'agit d'analyser l'intrusion, de stopper l'exfiltration de données critiques, de nettoyer l'infrastructure et de rassurer les instances dirigeantes via une communication de crise maîtrisée.

OUTILS, CONCEPTS & FRAMEWORKS UTILISÉS

Techniques d'Attaque Avancées (APT / MITRE ATT&CK)

Accès Initial & Évasion : Spear Phishing, Typosquatting (usurpation du domaine microsooft.com) et HTML Smuggling pour contourner les filtres proxy.

Persistance & Élévation de Privilèges : Modification de clés de registre (Run) pour exécuter un faux binaire système (Bginfo.exe / Masquerading) et utilisation d'un compte de service pour injecter un backdoor dans le groupe critique Domain Admins.

Défense et Analyse Réseau

Exfiltration Furtive (Data Leak) : Détection et analyse de DNS Tunneling (encodage des données volées via des requêtes DNS over TCP sur le port 53).

Network Defense (IPS/IDS) : Création de règles de blocage réseau ciblées via Snort.

COMPÉTENCES ACQUISES & DÉPLOYÉES

(Hard & Soft Skills SOC)

Forensic et Rétro-ingénierie d'Exfiltration (Hard Skills)

Analyse de flux furtif : Capacité à décortiquer une technique de vol de données silencieuse.

Cas pratique réalisé : Identification d'un flux DNS suspect. Extraction des sous-domaines, puis conversion du payload depuis le format Hexadécimal vers l'ASCII pour prouver avec exactitude la nature de la fuite : un dump complet des comptes Active Directory et des mots de passe administrateurs en clair.

Endiguement et Éradication Systémique (Hard Skills)

Disaster Recovery : Capacité à formuler et appliquer un plan de reprise d'activité immédiat.

Cas pratique réseau : Écriture d'une règle SNORT personnalisée (block tcp $HOME_NET 53 -> 183.251.167.28 53) pour couper net le tunnel d'exfiltration.

Cas pratique système : Planification du nettoyage chirurgical de l'Active Directory (suppression des comptes pirates, destruction des tâches planifiées, nettoyage de la base de registre) couplée à un "Force Reset" massif des comptes compromis.

Gestion de Crise et Restitution Executive (Soft Skills)

Traduction stratégique : Capacité à traduire l'urgence technique en langage stratégique pour les niveaux de direction (C-Level).

Cas pratique réalisé : Création d'un support de soutenance et présentation orale. Vulgarisation par l'analogie (ex: expliquer le Tunneling DNS aux métiers en le comparant à un découpage de données envoyé en "code morse") pour justifier les coupures de services.

LIVRABLES

[x] Rapports d'Investigation et de Remédiation (PDF / TheHive) : Exports détaillés du SIRP attestant de l'identification de la Kill Chain complète et de la liste exacte des actions curatives (Équipes Système, Réseau, et Active Directory).

[x] Règle de Détection/Blocage (Code) : Fichier contenant la règle Snort opérationnelle pour neutraliser la fuite de données (Drop du flux TCP/53).

[AD_P9_appuierez-vous-sur-le-bouton-rouge_2026-01-19T084129.zip](https://github.com/user-attachments/files/26643519/AD_P9_appuierez-vous-sur-le-bouton-rouge_2026-01-19T084129.zip)


[x] Support de Présentation de Crise (PPTX) : Diaporama exécutif à destination de la direction de l'entreprise (Résumé de la situation, chronologie technique, impacts et mesures de remédiation).
