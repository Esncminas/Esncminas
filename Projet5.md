<div align="center">
<h1>PROJET 5 | Endiguement et Réponse à Incident</h1>
<p><i>Contenez vos premiers incidents</i></p>
</div>

OBJECTIF DU PROJET

Réponse Active (IR) : Ce projet marque le passage de l'analyse (Blue Team) à la réaction active (Incident Response). L'objectif est d'apprendre à endiguer la propagation d'une cyberattaque au sein du Système d'Information (SI) d'une banque internationale. Il s'agit de concevoir des plans d'action stricts respectant les procédures SOC et d'appliquer des mesures de remédiation techniques automatisées (via API) pour neutraliser la menace.

OUTILS, CONCEPTS & FRAMEWORKS UTILISÉS

Méthodologies & Menaces

Réponse à Incident : Application stricte des phases du NIST et du SANS (Identification, Containment/Confinement, Eradication, Recovery/Restauration).

Cybermenaces Avancées : Étude des ransomwares (ex: affiliés Lockbit) et des compromissions Active Directory (attaques sur les tickets Kerberos type Kerberoasting, et vol d'identifiants via des outils offensifs comme Mimikatz).

Technologies & Automatisation

Technologies d'Endiguement : EDR (Endpoint Detection & Response), Firewalls, WAF (Web Application Firewall).

Programmation API (Python) : Automatisation des blocages réseau via la bibliothèque requests (Appels API REST en méthode POST).

COMPÉTENCES ACQUISES & DÉPLOYÉES

(Hard & Soft Skills SOC)

Investigation et Remédiation Système (Hard Skills)

Analyse de compromission : Capacité à analyser une compromission complexe (ex: exécution de yolokatz.exe / Mimikatz sur un contrôleur de domaine).

Cas pratique réalisé : Définition d'un plan d'éradication complet suite à une attaque Kerberoasting (Isolation de la machine, réinitialisation du compte de service compromis srv_database_app01, blocage du hash malveillant dans l'EDR, et audit des autres comptes à privilèges).

Endiguement Réseau Automatisé / SOAR (Hard Skills)

Interaction programmatique : Capacité à dialoguer programmatiquement avec des équipements de sécurité pour gagner un temps précieux en situation de crise.

Cas pratique réalisé : Développement de scripts Python pour se connecter à l'API du Firewall de l'entreprise et bannir instantanément (Blacklist) une IP de Command & Control (C2) liée au ransomware Lockbit, ainsi qu'une liste massive d'IPs malveillantes ciblant le WAF.

Gestion de Crise et Prise de Décision (Soft Skills)

Adaptation de la réponse : Capacité à adapter la réponse selon la criticité.

Cas pratique réalisé : Différenciation entre une attaque critique (Vrai Positif nécessitant un blocage immédiat) et une simple violation de la politique de sécurité (détection d'un scan Nmap légitime mais non déclaré par un administrateur interne), nécessitant de la sensibilisation plutôt qu'une isolation brutale.

LIVRABLES

[x] Plan d'Action de Remédiation (PDF) : Document formel d'investigation traitant plusieurs alertes (Scan Nmap, Kerberoasting), incluant la cartographie MITRE ATT&CK (TA0007, T1046), l'analyse du contexte et la liste numérotée des actions de confinement, d'éradication et de durcissement (Tuning SIEM).

[x] Scripts d'Automatisation Firewall (Python) : Codes source opérationnels démontrant la capacité à envoyer des payloads JSON (Action: "block") vers l'API d'un pare-feu pour neutraliser des adresses IP suspectes en temps réel.

[AD_P5_contenez-vos-premiers-incidents-1_2025-05-09T072301.zip](https://github.com/user-attachments/files/26643457/AD_P5_contenez-vos-premiers-incidents-1_2025-05-09T072301.zip)

