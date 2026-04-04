<div align="center">
  <h1>Hi 👋, I'm [Ton Prénom] [Ton Nom]</h1>
  <h3>🛡️ Analyste SOC | Ingénieur SecOps en devenir</h3>
  
  <p>
    <img src="https://img.shields.io/badge/SecOps-10B981?style=for-the-badge&logo=shield&logoColor=white" alt="SecOps"/>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
    <img src="https://img.shields.io/badge/Make.com-8B5CF6?style=for-the-badge" alt="Make"/>
    <img src="https://img.shields.io/badge/CTI-EF4444?style=for-the-badge&logo=hackthebox&logoColor=white" alt="CTI"/>
  </p>
  
  > **Mission :** Automatiser la défense, réduire l'"Alert Fatigue" des équipes SOC et transformer le bruit des incidents en décisions qualifiées.
</div>

---

## 🚀 Projet Majeur : SOAR Phishing Analyzer

**Le Problème :** Les équipes SOC sont saturées par les signalements d'e-mails suspects (Alert Fatigue) et perdent un temps précieux sur des qualifications manuelles répétitives.
**La Solution :** Conception et déploiement d'une architecture SOAR hybride 100% automatisée (Ingestion ➔ Forensics ➔ CTI ➔ Scoring IA ➔ Rapport).

* ⚙️ **Design Pattern "Scatter-Gather" :** Parallélisation des flux d'analyses (Fichiers, IPs, URLs), stockage en mémoire, et convergence pour générer un score de risque unique.
* 🐍 **Analyse Forensique (Micro-service) :** Script Python serverless pour extraire l'IP source réelle (contournement des IP privées) et valider la cryptographie (SPF/DKIM).
* 🔀 **Aiguillage Dynamique :** Routage intelligent via filtre MIME (Analyse QR Codes vs. Malware Binaires).
* 🧠 **IA & Threat Intelligence :** Intégration d'APIs (AbuseIPDB, URLScan) et analyse sémantique par LLM (détection d'urgence et protection anti-Prompt Injection).

### 🗺️ Architecture de Détection

```mermaid
graph LR
  classDef rootStyle fill:#2563EB,stroke:#fff,stroke-width:2px,color:#fff,font-weight:bold,font-size:14px;
  classDef nodeStyle fill:#F8FAFC,stroke:#CBD5E1,stroke-width:1px,color:#1E293B;

  ROOT("🛡️ SOAR Phishing Analyzer"):::rootStyle
  
  ROOT --> INGEST["📥 1. Ingestion & Parsing<br/>(Watch Emails, Regex)"]:::nodeStyle
  ROOT --> IA["🧠 2. Analyse Sémantique IA<br/>(Prompt Guards)"]:::nodeStyle
  ROOT --> FOR["🔎 3. Moteurs Forensics<br/>(Python, AbuseIPDB, URLScan)"]:::nodeStyle
  ROOT --> REP["📊 4. Consolidation<br/>(Score Mathématique & Reporting HTML)"]:::nodeStyle
````
Expertise,Niveau,Compétences Validées

Architecture SOAR & Automatisation,█████████░ 90%,
--> "Modélisation logique, gestion des erreurs natives, exécution parallèle, manipulation de variables en mémoire."
Forensique E-mail & Threat Intel,████████░░ 80%,
--> "Parsing d'entêtes complexes (Headers EML), typage MIME, enrichissement IoC (CTI)."
Programmation Python & API REST,███████░░░ 70%,
--> "Scripting (Regex), requêtes HTTP synchrones (Webhooks), sérialisation et parsing JSON."

Autres Projets Techniques
<details>
<summary><b>🛡️ Audit de vulnérabilités et Pentest Web (Cliquez pour dérouler)</b></summary>


Compétences : Méthodologie OWASP, cartographie Nmap, exploitation via Burp Suite, rédaction de plan de remédiation.

Livrable : 🔗 Lien vers le rapport d'audit anonymisé

</details>

<details>
<summary><b>👁️ Déploiement d'un SIEM et Supervision Réseau (Cliquez pour dérouler)</b></summary>

Compétences : Installation et configuration de Wazuh, création de règles de détection d'intrusions (Blue Team).

Livrable : 🔗 Lien vers le Dashboard de supervision

</details>

Expériences & Soft Skills
[Mois Année – Mois Année] | [Intitulé du poste] chez [Nom de l'entreprise]

Missions : Résolution des tickets d'incidents informatiques niveau 1 & 2.
Soft Skills : Relation client, gestion du stress, communication inter-équipes.

[Mois Année – Mois Année] | [Intitulé du poste] chez [Nom de l'entreprise]
Missions : Déploiement de solutions logicielles, sensibilisation des utilisateurs.
Soft Skills : Pédagogie, vulgarisation technique.

🇬🇧 Anglais Technique & Professionnel (B2/C1)
La maîtrise de l'anglais technique est le cœur de mon environnement de travail (débruitage de logs, ingénierie) :

📚 Recherche & Ingénierie : Intégration d'outils complexes exclusivement via des documentations anglophones (Pipedream Developer Docs, RFC standards mondiaux des e-mails).
🔧 Troubleshooting : Interprétation des codes d'erreurs serveurs (Unprocessable Entity, BundleValidationError) et échanges sur des forums spécialisés (StackOverflow).
💻 Standardisation : Nommage systématisé des variables (rawBodyContent, ip_source) et structuration des flux JSON selon les conventions de la scène tech internationale.

<div align="center">
<i>Prêt à relever de nouveaux défis en cybersécurité.</i>



<a href="https://www.google.com/search?q=https://linkedin.com/in/[ton-profil]" target="_blank"><img src="https://www.google.com/search?q=https://img.shields.io/badge/LinkedIn-0077B5%3Fstyle%3Dfor-the-badge%26logo%3Dlinkedin%26logoColor%3Dwhite" alt="LinkedIn"/></a>
<a href="mailto:[ton-email@exemple.com]"><img src="https://www.google.com/search?q=https://img.shields.io/badge/Contact-D14836%3Fstyle%3Dfor-the-badge%26logo%3Dgmail%26logoColor%3Dwhite" alt="Email"/></a>
</div>
