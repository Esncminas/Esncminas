<div align="center">
  <h1>🛑 PROJET 5 | Contenez vos premiers incidents </h1>
  <p><b>Contenez vos premiers incidents (Incident Response & API)</b></p>

  <img src="https://img.shields.io/badge/STATUT-TERMINÉ-success?style=for-the-badge&logo=checkmarx" alt="Statut" />
  <img src="https://img.shields.io/badge/THÈME-INCIDENT_RESPONSE-blue?style=for-the-badge&logo=fortinet" alt="Thème" />
  <img src="https://img.shields.io/badge/NIVEAU-OPÉRATIONNEL-orange?style=for-the-badge" alt="Niveau" />
</div>

---

##  <u>OBJECTIF DU PROJET</u>

> **Réponse Active (IR)**
> Ce projet marque le passage de l'analyse passive (Blue Team) à la **réaction active**. L'objectif est d'apprendre à endiguer la propagation d'une cyberattaque au sein du Système d'Information (SI) d'une banque internationale. Il s'agit de concevoir des plans d'action stricts respectant les procédures SOC et d'appliquer des <u>mesures de remédiation techniques automatisées</u> (via API) pour neutraliser la menace de manière chirurgicale.

---

##  <u>OUTILS, CONCEPTS & FRAMEWORKS</u>

La réponse à incident nécessite de maîtriser à la fois les procédures d'urgence et les technologies de blocage :

| Catégorie | Outils & Concepts | Application & Cas d'usage SOC |
| :--- | :--- | :--- |
| 📜 **Méthodologies** | **NIST & SANS (IR)** | Application stricte des phases : Identification, Confinement, Éradication, Restauration. |
| 🦠 **Cybermenaces** | **Ransomware & AD** | Étude d'affiliés Lockbit et des compromissions Active Directory (Kerberoasting, Mimikatz). |
| 🛡️ **Technologies** | **EDR, WAF, Firewalls** | Utilisation des équipements de sécurité périmétriques et *endpoints* pour l'endiguement. |
| 🐍 **Automatisation** | **Python (API REST)** | Automatisation des blocages réseau via la bibliothèque `requests` (Appels POST). |

---

##  <u>COMPÉTENCES ACQUISES & DÉPLOYÉES</u>
*(Hard & Soft Skills SOC)*

###  <u>Investigation et Remédiation Système (Hard Skills)</u>
* **Analyse de compromission** : Capacité à analyser une attaque complexe (ex: exécution de l'outil offensif `yolokatz.exe` / Mimikatz sur un contrôleur de domaine).
* **Éradication (Kerberoasting)** : Définition d'un plan d'action complet suite au vol d'identifiants (Isolation de la machine, réinitialisation du compte de service `srv_database_app01`, blocage du hash malveillant dans l'EDR, et audit des autres comptes à privilèges).

###  <u>Endiguement Réseau Automatisé / SOAR (Hard Skills)</u>
* **Interaction programmatique** : Capacité à dialoguer directement avec des équipements de sécurité pour gagner un temps précieux en situation de crise.
* **Cas pratique d'endiguement** : Développement de scripts Python pour se connecter à <u>l'API du Firewall</u> de l'entreprise et bannir instantanément (*Blacklist*) une IP de *Command & Control* (C2) liée au ransomware Lockbit, ainsi qu'une liste massive d'IPs malveillantes ciblant le WAF.

###  <u>Gestion de Crise et Prise de Décision (Soft Skills)</u>
* **Adaptation de la réponse** : Différenciation critique entre un Vrai Positif nécessitant un blocage immédiat et une simple violation de politique de sécurité (ex: détection d'un scan Nmap interne légitime mais non déclaré). Cette dernière nécessite de la <u>sensibilisation plutôt qu'une isolation brutale</u>.

---

## 📦 <u>LIVRABLES</u>

- [x] **Plan d'Action de Remédiation (PDF)** : Document formel d'investigation traitant plusieurs alertes (Scan Nmap, Kerberoasting), incluant la cartographie MITRE ATT&CK (TA0007, T1046) et la liste numérotée des actions de confinement, d'éradication et de durcissement.
- [x] **Scripts d'Automatisation Firewall (Python)** : Codes source opérationnels démontrant la capacité à envoyer des *payloads* JSON (Action: `"block"`) vers l'API d'un pare-feu pour neutraliser des adresses IP suspectes en temps réel.

<br>

<div align="center">
  <a href="https://github.com/user-attachments/files/26643457/AD_P5_contenez-vos-premiers-incidents-1_2025-05-09T072301.zip">
    <img src="https://img.shields.io/badge/TÉLÉCHARGER_L'ARCHIVE_DU_PROJET-ZIP-brightgreen?style=for-the-badge&logo=github" alt="Download" />
  </a>
</div>

---
<p align="center"><i>Réalisé dans le cadre de la certification Analyste SOC</i></p>
