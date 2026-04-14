<div align="center">
<h1>PROJET 8 | Limitez les faux positifs</h1>
<p><i>Optimisez en continu le système de gestion de connaissances interne</i></p>
</div>

OBJECTIF DU PROJET

Amélioration Continue et Tuning : L'objectif de ce projet est d'adopter une posture d'amélioration continue au sein du SOC d'une entreprise de vente en ligne. Face au risque d'"Alert Fatigue", il s'agit d'optimiser les règles de détection (Tuning) pour réduire drastiquement les Faux Positifs, et de capitaliser sur les retours d'expérience (Lessons Learned) pour enrichir la base de connaissances interne (Knowledge Management) via la rédaction et l'amélioration de procédures de réponse à incident (Playbooks).

OUTILS, CONCEPTS & FRAMEWORKS UTILISÉS

Ingénierie de Détection (Detection Engineering)

Format Sigma : Utilisation du standard Sigma (format YAML) pour l'écriture et l'optimisation de règles de détection agnostiques.

SIEM Elastic : Création de règles et gestion des listes d'exceptions (Exception Lists) directement dans la plateforme Elasticsearch.

Capitalisation

Knowledge Management : Élaboration de Fiches Réflexes (Playbooks/SOPs) pour standardiser la réponse des analystes L1 face à des menaces récurrentes.

Rule Lifecycle : Capacité à auditer une bibliothèque de règles de sécurité et à écarter celles générant trop de bruit ou relevant de la simple supervision IT.

COMPÉTENCES ACQUISES & DÉPLOYÉES

(Hard & Soft Skills SOC)

Tuning et Réduction des Faux Positifs (Hard Skills)

Affinage de règles : Capacité à affiner une règle de détection pour la rendre "silencieuse" sur les comportements légitimes tout en restant intraitable sur les menaces.

Cas pratique (Sigma) : Optimisation d'une règle détectant les attaques Brute-Force (EventID 4625). Ajout de filtres d'exclusion pour ignorer les comptes de service connus (svc_test) et les comptes déjà verrouillés.

Cas pratique (Elastic) : Création d'une règle de détection de "Scan de ports" incluant une liste d'exceptions (Whitelist) pour autoriser l'adresse IP du scanner de vulnérabilités interne (192.168.9.10), évitant ainsi le déclenchement intempestif du SIEM.

Évaluation Stratégique de la Détection (Hard Skills)

Audit de pertinence : Capacité à justifier le rejet de règles inadaptées à un SOC.

Cas pratique réalisé : Rejet justifié d'une règle d'alerte sur un "Espace disque à 70%", requalifiée en incident de supervision système (Monitoring IT) et non en incident de cybersécurité.

Capitalisation et Vulgarisation (Soft Skills & Rigueur)

Structuration de l'information : Capacité à structurer la connaissance pour faciliter le travail de l'équipe (Handover/Onboarding).

Cas pratique réalisé : Amélioration d'une fiche d'investigation Wazuh (analyse d'élévation de privilèges via les champs systèmes TokenElevationType et mandatoryLabel) et création intégrale d'un Playbook de qualification de Phishing.

LIVRABLES

[x] Rapport d'optimisation de la détection : Document d'expertise justifiant la sélection ou le rejet technique de 5 règles de détection proposées.

[x] Règles de Détection Optimisées (Code) : Fichier de règle générique (.yaml) codé au standard Sigma ciblant les échecs d'authentification multiples, et export de règle SIEM Elastic (.ndjson) incluant la gestion d'une liste d'exceptions.

[x] Base de Connaissances / Playbooks : Livrables opérationnels comprenant une fiche réflexe entièrement créée (Traitement de Phishing) et une fiche améliorée techniquement (Investigation de processus via Wazuh).

[AD_P8_limitez-les-faux-positifs_2025-10-23T130258.zip](https://github.com/user-attachments/files/26643480/AD_P8_limitez-les-faux-positifs_2025-10-23T130258.zip)
