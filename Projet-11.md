<div align="center">
  <h1>SOAR Phishing Analyzer (Make.com + IA)</h1>
  <p><b>Pipeline SecOps 100% automatisé pour l'analyse Forensics et Sémantique d'e-mails suspects.</b></p>

  <p>
    <img src="https://img.shields.io/badge/Orchestration-Make.com-8B5CF6?style=for-the-badge" alt="Make"/>
    <img src="https://img.shields.io/badge/AI_Engine-Google_Gemini-F59E0B?style=for-the-badge&logo=google" alt="Gemini"/>
    <img src="https://img.shields.io/badge/Threat_Intel-REST_APIs-3B82F6?style=for-the-badge" alt="APIs"/>
    <img src="https://img.shields.io/badge/Data-JSON_&_Regex-10B981?style=for-the-badge" alt="Data"/>
  </p>
</div>

---

## Contexte & Objectif

Les équipes SOC (Security Operations Center) souffrent d'**"Alert Fatigue"** face à la masse d'e-mails suspects signalés par les collaborateurs. La qualification manuelle de ces alertes est répétitive et chronophage.

**La Solution :** J'ai architecturé ce SOAR (Security Orchestration, Automation, and Response) pour automatiser l'analyse de bout en bout. Il combine des moteurs Forensics traditionnels (réputation IP, sandboxing) avec une **Intelligence Artificielle (LLM)** pour comprendre le contexte sémantique de l'attaque.

---

## Architecture de Détection

L'architecture repose sur un design pattern *Scatter-Gather* : parallélisation des analyses et convergence vers un score unique.

```mermaid
graph LR
  classDef rootStyle fill:#2563EB,stroke:#fff,stroke-width:2px,color:#fff,font-weight:bold,font-size:14px;
  classDef nodeStyle fill:#F8FAFC,stroke:#CBD5E1,stroke-width:1px,color:#1E293B;

  ROOT("🛡️ SOAR Phishing Analyzer"):::rootStyle
  
  ROOT --> INGEST["📥 1. Ingestion & Parsing<br/>(Watch Emails, Regex)"]:::nodeStyle
  ROOT --> IA["🧠 2. Analyse Sémantique IA<br/>(Gemini + Prompt Guards)"]:::nodeStyle
  ROOT --> FOR["🔎 3. Moteurs Forensics<br/>(AbuseIPDB, URLScan)"]:::nodeStyle
  ROOT --> REP["📊 4. Consolidation<br/>(Calcul Mathématique & HTML)"]:::nodeStyle
```

<mark>Fonctionnalités Techniques Clés</mark><br>

**<ins>1. Moteur Sémantique IA (Google Gemini)</ins>**<br><br>
**Détection d'Ingénierie Sociale :** Analyse du corps de l'e-mail pour détecter les sentiments d'urgence, la coercition ou l'usurpation d'identité.<br>
**Sécurité "Prompt Guard" :** Implémentation de garde-fous stricts dans le prompt pour empêcher les attaques par Prompt Injection (où un attaquant cacherait des instructions invisibles dans l'e-mail pour tromper l'IA).<br>
**Formatage JSON :** Contrainte de l'IA pour générer une réponse 100% JSON avec un verdict (SAFE, SUSPICIOUS, MALICIOUS), un score sur 50 et une justification.<br>

**<ins>2. Moteurs Forensics & Routage Dynamique</ins>**<br><br>
**Extraction d'IOCs :** Utilisation d'Expressions Régulières (Regex) avancées pour isoler les adresses IP, les domaines et les URLs cachées.<br>
**Aiguillage MIME :** Séparation dynamique des flux selon le type de pièce jointe (analyse visuelle pour les QR Codes, analyse binaire pour les PDF/ZIP).<br>
**Threat Intelligence :** Interrogation synchronisée des API AbuseIPDB et Urlscan.io.<br>

**<ins>3. Consolidation & Triage Automatisé</ins>**<br><br>
**Calculateur de Menace :** Utilisation de fonctions mathématiques (parseNumber, ifempty) pour agréger les scores isolés de chaque branche en un Score de Menace Global sur 100.
**Génération de Rapport HTML :** Création d'un template HTML dynamique injectant les variables pour restituer un tableau de bord lisible directement dans la boîte mail des analystes SOC.

📸 Aperçu du Projet
<table width="100%">
<tr>
<td width="50%" align="center">
<b>Arbre d'Orchestration (Make)</b>

<img width="1295" height="769" alt="Capture d’écran 2026-04-04 173242" src="https://github.com/user-attachments/assets/b00b6f79-0b92-4f3c-bb41-3e39a6d33521" />

<i>Vue globale du pipeline SecOps.</i>
</td>
<td width="50%" align="center">
<b>Rapport d'Investigation Généré</b><br>

<img width="709" height="730" alt="Capture d’écran 2026-04-04 173109" src="https://github.com/user-attachments/assets/ece6196c-99ca-45f4-952f-507661b52e3a" />



<i>Le résultat final exploitable par le SOC.</i>
</td>
</tr>
</table>

<div align="center">
<i>Projet conçu dans le cadre de mon portfolio technique d'Analyste Cybersécurité.</i>
</div>
