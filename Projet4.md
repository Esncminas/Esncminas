<div align="center">
<h1>PROJET 4 | Scripts Python de Réponse à Incident</h1>
<p><i>Rédigez vos premiers scripts en Python</i></p>
</div>

OBJECTIF DU PROJET

Automatisation de la Réponse (IR) : Ce projet introduit la programmation comme levier fondamental pour l'automatisation de la réponse aux incidents (Incident Response). L'objectif est de concevoir un outil en Python capable d'analyser une arborescence de serveurs web clients, de détecter des Web Shells ou scripts malveillants basés sur des indicateurs de compromission (IoC), et d'appliquer une mesure de remédiation automatisée (Neutralisation).

OUTILS, CONCEPTS & FRAMEWORKS UTILISÉS

Langage & Environnement

Python 3 : Utilisation de la bibliothèque standard os pour les interactions avec le système de fichiers.

Concepts SecOps

IoC Matching : Recherche d'Indicateurs de Compromission statiques (noms de fichiers spécifiques) et dynamiques (adresses IP d'un serveur de Commande & Contrôle caché dans le code).

Defanging / Neutralisation : Technique consistant à rendre une menace inopérante sans pour autant détruire l'artefact.

COMPÉTENCES ACQUISES & DÉPLOYÉES

(Hard & Soft Skills SOC)

Développement d'outils de sécurité (Hard Skills)

Création de script d'investigation : Développement itératif d'outils d'analyse (Scripts 1 à 4).

Analyse de fichiers : Capacité à parcourir récursivement des répertoires (os.walk), lire et décortiquer le contenu des fichiers pour y traquer une adresse IP malveillante (8.13.193.9) ou identifier un préfixe suspect (xmc6_).

Remédiation et Préservation des Preuves (Hard Skills)

Gestion d'incident (NIST) : Maîtrise des concepts de réponse à incident (Phases Containment & Eradication).

Cas pratique réalisé : Prise de décision technique cruciale via l'implémentation d'une fonction pour renommer les fichiers infectés (ajout de l'extension .txt) plutôt que de les supprimer. Cela casse l'exécution côté serveur (ex: neutralisation d'un fichier .php) tout en préservant le code source intact pour l'équipe d'investigation numérique (Forensic / Reverse Engineering).

Logique Algorithmique (Soft Skills)

Décomposition de problèmes : Capacité à décomposer un problème complexe en sous-tâches simples (Lister les fichiers -> Trouver les noms suspects -> Lire le contenu interne -> Appliquer la modification).

LIVRABLES

[x] Code Source (Python) : Script complet (Script 4.py) intégrant la gestion des erreurs (try/except), la détection multicritères (nom + contenu) et la neutralisation automatisée des menaces.

[x] Note d'ingénierie / Documentation : Document PDF justifiant l'approche algorithmique choisie, les conditions de détection, et l'explication stratégique de la neutralisation par renommage (.txt) pour la conservation des preuves.

[AD_P4_redigez-vos-premiers-scripts-en-python_2025-04-11T080357.zip](https://github.com/user-attachments/files/26643404/AD_P4_redigez-vos-premiers-scripts-en-python_2025-04-11T080357.zip)

