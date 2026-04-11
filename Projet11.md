SOAR Phishing Analyzer (Make.com + IA)
Pipeline SecOps 100% automatisé pour l'analyse Forensics et Sémantique d'e-mails suspects.

Make Gemini APIs Data

Contexte & Objectif
Les équipes SOC (Security Operations Center) souffrent d'"Alert Fatigue" face à la masse d'e-mails suspects signalés par les collaborateurs. La qualification manuelle de ces alertes est répétitive et chronophage.

La Solution : J'ai architecturé ce SOAR (Security Orchestration, Automation, and Response) pour automatiser l'analyse de bout en bout. Il combine des moteurs Forensics traditionnels (réputation IP, sandboxing) avec une Intelligence Artificielle (LLM) pour comprendre le contexte sémantique de l'attaque.

Architecture de Détection
L'architecture repose sur un design pattern Scatter-Gather : parallélisation des analyses et convergence vers un score unique.


Fonctionnalités Techniques Clés

1. Moteur Sémantique IA (Google Gemini)

Détection d'Ingénierie Sociale : Analyse du corps de l'e-mail pour détecter les sentiments d'urgence, la coercition ou l'usurpation d'identité.
Sécurité "Prompt Guard" : Implémentation de garde-fous stricts dans le prompt pour empêcher les attaques par Prompt Injection (où un attaquant cacherait des instructions invisibles dans l'e-mail pour tromper l'IA).
Formatage JSON : Contrainte de l'IA pour générer une réponse 100% JSON avec un verdict (SAFE, SUSPICIOUS, MALICIOUS), un score sur 50 et une justification.

2. Moteurs Forensics & Routage Dynamique

Extraction d'IOCs : Utilisation d'Expressions Régulières (Regex) avancées pour isoler les adresses IP, les domaines et les URLs cachées.
Aiguillage MIME : Séparation dynamique des flux selon le type de pièce jointe (analyse visuelle pour les QR Codes, analyse binaire pour les PDF/ZIP).
Threat Intelligence : Interrogation synchronisée des API AbuseIPDB et Urlscan.io.

ins>3. Consolidation & Triage Automatisé3. Consolidation & Triage Automatisé

Calculateur de Menace : Utilisation de fonctions mathématiques (parseNumber, ifempty) pour agréger les scores isolés de chaque branche en un Score de Menace Global sur 100. Génération de Rapport HTML : Création d'un template HTML dynamique injectant les variables pour restituer un tableau de bord lisible directement dans la boîte mail des analystes SOC.

📸 Aperçu du Projet

Arbre d'Orchestration (Make) Capture d’écran 2026-04-04 173242
Vue globale du pipeline SecOps.

Rapport d'Investigation Généré
Capture d’écran 2026-04-04 173109
Le résultat final exploitable par le SOC.

Projet conçu dans le cadre de mon portfolio technique d'Analyste Cybersécurité.
