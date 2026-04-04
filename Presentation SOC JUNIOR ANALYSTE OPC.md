<div align="center">
  <h1>Salut 👋,Je m'appel Adrien DUCTANE</h1>
  <h3>🛡️ Analyste Junior SOC | Ingénieur SecOps en devenir</h3>
  
  <p>
    <img src="https://img.shields.io/badge/SecOps-10B981?style=for-the-badge&logo=shield&logoColor=white" alt="SecOps"/>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
    <img src="https://img.shields.io/badge/Make.com-8B5CF6?style=for-the-badge" alt="Make"/>
    <img src="https://img.shields.io/badge/CTI-EF4444?style=for-the-badge&logo=hackthebox&logoColor=white" alt="CTI"/>
  </p>
  
  > **Mission :** Automatiser la défense, réduire l'"Alert Fatigue" des équipes SOC et transformer le bruit des incidents en décisions qualifiées.
</div>

---

##  Projet Majeur : SOAR Phishing Analyzer

**Le Problème :** Les équipes SOC sont saturées par les signalements d'e-mails suspects (Alert Fatigue) et perdent un temps précieux sur des qualifications manuelles répétitives.
**La Solution :** Conception et déploiement d'une architecture SOAR hybride 100% automatisée (Ingestion ➔ Forensics ➔ CTI ➔ Scoring IA ➔ Rapport).

* **Design Pattern "Scatter-Gather" :** Parallélisation des flux d'analyses (Fichiers, IPs, URLs), stockage en mémoire, et convergence pour générer un score de risque unique.
* **Analyse Forensique (Micro-service) :** Script Python serverless pour extraire l'IP source réelle (contournement des IP privées) et valider la cryptographie (SPF/DKIM).
* **Aiguillage Dynamique :** Routage intelligent via filtre MIME (Analyse QR Codes vs. Malware Binaires).
* **IA & Threat Intelligence :** Intégration d'APIs (AbuseIPDB, URLScan) et analyse sémantique par LLM (détection d'urgence et protection anti-Prompt Injection).

###  Architecture de Détection

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
<div align="center">
  <a href="[https://github.com/ton-pseudo/projet-1](https://github.com/Esncminas/SOAR-PHISING-ANALYSTE-MAKE-IA)">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=ton-pseudo&repo=projet-1&theme=radical" width="400" />
  </a>
</div>

**<mark>Expertise,Niveau,Compétences Validées</mark>**

Architecture SOAR & Automatisation,█████████░ 90%,<br> 
--> "Modélisation logique, gestion des erreurs natives, exécution parallèle, manipulation de variables en mémoire."<br> 
Forensique E-mail & Threat Intel,████████░░ 80%,<br> 
--> "Parsing d'entêtes complexes (Headers EML), typage MIME, enrichissement IoC (CTI)."<br> 
Programmation Python & API REST,███████░░░ 70%,<br> 
--> "Scripting (Regex), requêtes HTTP synchrones (Webhooks), sérialisation et parsing JSON."<br> 

**<mark>Autres Projets Techniques</mark>**
<details>
<summary><b> Audit de vulnérabilités et Pentest Web</b></summary>
Compétences : <br>
  ◼️ Méthodologie OWASP,<br> 
  ◼️ cartographie Nmap,<br>
  ◼️ rédaction de plan de remédiation.<br>
</details>

<details>
<summary><b> Déploiement d'un SIEM et Supervision Réseau</b></summary>
Compétences :<br> 
  ◼️ Installation et configuration de Wazuh,<br>
  ◼️ Utilisation THEHIVE & Cortex<br>
  ◼️ création de règles de détection d'intrusions (Blue Team).<br>
</details>

**<mark>Expériences & Soft Skills</mark>**

◼️ Projets formation SOC : <br>
Missions : Résolution des tickets d'incidents informatiques niveau 1 & 2.
Soft Skills : Relation client, gestion du stress, communication inter-équipes.

◼️ Projets formation SOC :<br> 
Missions : Déploiement de solutions logicielles, sensibilisation des utilisateurs.
Soft Skills : Pédagogie, vulgarisation technique.

◼️ Anglais Technique & Professionnel (B2/C1)<br>
La maîtrise de l'anglais technique est le cœur de mon environnement de travail (débruitage de logs, ingénierie) :

<mark>Recherche & Ingénierie</mark> : Intégration d'outils complexes exclusivement via des documentations anglophones (Pipedream Developer Docs, RFC standards mondiaux des e-mails).<br>
<mark>Troubleshooting</mark> : Interprétation des codes d'erreurs serveurs (Unprocessable Entity, BundleValidationError) et échanges sur des forums spécialisés (StackOverflow).<br>
<mark>Standardisation</mark> : Nommage systématisé des variables (rawBodyContent, ip_source) et structuration des flux JSON selon les conventions de la scène tech internationale.<br>

## 👁️ Ma représentation du métier & Soft Skills

<table width="100%">
<tr>
<td width="50%" valign="top">
<h3>Évolution de ma vision (Retex)</h3>

<blockquote>
<p><b>AU DÉBUT DE MA FORMATION</b></p>
Je voyais l'analyste comme un opérateur posté devant un SIEM, réagissant manuellement aux alertes selon des procédures très strictes.
</blockquote>

<blockquote>
<p><b style="color:#10B981;">MA VISION AUJOURD'HUI</b></p>
C'est un métier d'ingénierie et d'automatisation. L'analyste moderne construit ses propres outils (SOAR) pour qualifier la menace et se concentrer sur l'investigation complexe.
</blockquote>
</td>

<td width="50%" valign="top">
<h3>Soft Skills travaillés</h3>

<p><b>Rigueur & Troubleshooting</b><br>
<sub>Recherche de pannes étape par étape face aux bugs de syntaxe mathématique ou de parsing Regex.</sub></p>

<p><b>Anglais Professionnel</b><br>
<sub>Exploitation fluide des documentations techniques API en anglais (Urlscan, AbuseIPDB).</sub></p>
</td>
</tr>
</table>


<div align="center">
<i>Prêt à relever de nouveaux défis en cybersécurité.</i>

