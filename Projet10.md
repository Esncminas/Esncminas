<div align="center">
<h1>PROJET 10 | Améliorez et automatisez la détection et le traitement des alertes </h1>
<p><i>Automatisez des détections d'alertes</i></p>
</div>

OBJECTIF DU PROJET

Automatisation et Réduction du MTTR : L'objectif de ce projet est de concevoir une architecture de sécurité automatisée pour une entreprise du secteur de l'aéronautique (secteur à très haute sensibilité). Face au volume croissant d'événements, le but est de réduire le temps de réponse aux incidents (MTTR) et d'éliminer les tâches manuelles répétitives des analystes. Le projet consiste à développer des tableaux de bord de détection avancés dans Splunk et à programmer des outils d'enrichissement sur-mesure (Cortex) orchestrés par un SOAR (n8n).

OUTILS, CONCEPTS & FRAMEWORKS UTILISÉS

Orchestration et Investigation

SOAR (n8n) : Utilisation de n8n pour créer des workflows automatisant le cycle de vie des alertes (réception par webhook, routage, enrichissement, clôture).

Cortex & TheHive : Développement d'Analyzers personnalisés pour enrichir automatiquement les observables (IoC) directement dans les tickets d'incidents.

Analyse et Développement

Splunk (SIEM) : Utilisation du langage SPL (Search Processing Language) pour la création de requêtes complexes et de Dashboards de supervision.

Programmation Python : Interaction avec l'Active Directory (bibliothèque ldap3) et avec des API REST externes (bibliothèque requests).

COMPÉTENCES ACQUISES & DÉPLOYÉES

(Hard & Soft Skills SOC)

Développement SecOps et Intégration d'API (Hard Skills)

Micro-services (Analyzers) : Capacité à coder des scripts Python pour connecter les outils de sécurité entre eux.

Cas pratique 1 (API Externe) : Développement d'un analyseur d'IP interrogeant l'API ip-api.com pour géolocaliser une adresse et générer automatiquement des "Taxonomies" visuelles dans TheHive (Pays, FAI, VPN).

Cas pratique 2 (LDAP) : Développement d'un analyseur LDAP capable d'interroger directement l'annuaire Active Directory de l'entreprise pour retrouver instantanément la description et le rôle de la machine ou de l'utilisateur compromis.

Création de Dashboards SIEM (Hard Skills)

Exploitation de la donnée : Capacité à exploiter la donnée brute pour mettre en évidence une compromission comportementale.

Cas pratique réalisé : Développement d'un Dashboard Splunk dédié à la détection des "Connexions inhabituelles" (Impossible Travel / Voyage Impossible). Utilisation de commandes SPL pour trier, géolocaliser (Geostats) et filtrer les utilisateurs se connectant depuis plusieurs continents de manière anormale.

Automatisation et Réduction du MTTA/MTTR (Soft Skills & Ingénierie)

Optimisation des processus : Le passage d'un enrichissement manuel (recherche de l'IP, puis recherche dans l'AD) à un workflow n8n 100% autonome permet aux analystes de se concentrer uniquement sur l'investigation à forte valeur ajoutée.

LIVRABLES

[x] Scripts d'Analyse Python (Cortex Analyzers) : Code source des analyseurs documentés (LDAP_Machine.py et IP_Check.py) incluant la gestion des requêtes, le parsing JSON, et la construction des labels de menace (Taxonomies).

[x] Captures d'Architecture (Dashboards & Workflows) : Preuves visuelles (Screenshots) du tableau de bord de supervision Splunk (carte de connexions, alertes critiques) et des flux de données automatisés au sein du SOAR n8n.

[AD_P10_ameliorez-et-automatisez-la-detection-et-le-traitement-des-alertes_2026-03-13T091601.zip](https://github.com/user-attachments/files/26643529/AD_P10_ameliorez-et-automatisez-la-detection-et-le-traitement-des-alertes_2026-03-13T091601.zip)
