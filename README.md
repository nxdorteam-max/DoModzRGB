# DoModz RGB

**Éclairage et ventilation réunis dans une application Windows en français, sans publicité.**

[Télécharger la dernière version](https://github.com/nxdorteam-max/DoModzRGB/releases/latest) · [Signaler un problème](https://github.com/nxdorteam-max/DoModzRGB/issues)

## Installation

1. Télécharger `DoModz-RGB-Setup-3.1.0.exe` depuis les versions publiées.
2. Lancer l’installateur et accepter la demande administrateur Windows.
3. Ouvrir DoModz RGB depuis le menu Démarrer ou son icône près de l’horloge.

Windows 10 version 2004 ou ultérieure / Windows 11, 64 bits. Les commandes matérielles nécessitent les droits administrateur et un contrôleur compatible. Les composants Microsoft Visual C++ nécessaires sont inclus. Le pilote officiel PawnIO peut être installé depuis le logiciel s’il manque ; une installation existante est réutilisée.

**La croix ferme la fenêtre, pas le logiciel.** DoModz RGB continue de gérer ses réglages en arrière-plan. Le menu de son icône permet de le rouvrir ou de **Quitter complètement**.

## Fonctionnalités

### Éclairage

- Couleur fixe, arc-en-ciel, respiration, réaction au son, couleur moyenne de l’écran et extinction.
- Luminosité et vitesse réglables, avec sélection des éclairages compatibles.
- Affectation des prises RGB/ARGB au ventirad ou au boîtier, en renseignant le branchement réel.
- Distinction entre un contrôleur de carte mère, une prise disponible et un éclairage effectivement configuré.

### Ventilation

- Profils **Silencieux**, **Normal**, **Turbo** et **courbe personnalisée**.
- Application d’un profil à toutes les commandes compatibles détectées.
- Régulation selon la température du processeur ou un capteur de carte mère.
- Courbe personnalisée aux points 35, 50, 65 et 80 °C ; interpolation entre les points.
- Protection thermique et restauration des commandes lors d’une fermeture complète ou d’une perte de liaison détectée.
- Ventilation AMD via l’interface officielle ADLX, avec vérification des réponses du pilote.

### Utilisation quotidienne

- Interface française bleu-violet et actualisation sans reconstruction complète des listes.
- Températures CPU/GPU, régimes des ventilateurs et historique des dix dernières minutes.
- Inventaire mémorisé : les appareils absents restent identifiés comme déconnectés.
- Démarrage en arrière-plan à la connexion Windows et restauration des profils enregistrés.
- Raccourcis Windows, désinstallation standard et conservation des réglages personnels.

### Mises à jour signées

DoModz recherche les mises à jour au démarrage et toutes les six heures. Il vérifie un manifeste signé **RSA-PSS / SHA-256**, puis l’empreinte et la taille de l’installateur. Une version modifiée ou plus ancienne que la version installée est refusée. Une notification propose l’installation ; les réglages sont conservés.

La clé privée de publication n’est pas distribuée. La signature des mises à jour est **distincte d’un certificat Windows Authenticode** : cette première version n’a pas de certificat d’éditeur Windows commercial et peut afficher « éditeur inconnu ».

## Compatibilité et limites

- La détection Windows d’un composant ne garantit pas la prise en charge de son RGB ou de ses commandes de ventilation.
- Le mode Silencieux réduit les vitesses à basse température ; il ne garantit pas une absence totale de bruit.
- Un répartiteur peut regrouper plusieurs ventilateurs derrière une seule commande.
- Un câble RGB/ARGB ne transmet généralement pas le modèle du ventirad. Le nombre de LED et le branchement doivent alors être renseignés.
- Les capteurs de carte mère dont l’emplacement est inconnu ne sont pas présentés comme une mesure certaine de la température du boîtier.
- Le RGB de la **GIGABYTE RX 7600 XT révision PCI 242A** nécessite encore l’outil constructeur. Sa ventilation est prise en charge via ADLX. Plusieurs GPU AMD simultanés ne sont pas pris en charge par ce connecteur.
- Les mécanismes de restauration ne garantissent pas la récupération après une défaillance de Windows ou du pilote.

## Confidentialité et licences

Les paramètres et l’inventaire restent sur le PC, dans `%LOCALAPPDATA%\DoModzRGB`. L’application contacte GitHub pour les mises à jour, sans envoyer l’inventaire matériel.

Ce dépôt distribue les installateurs, la documentation et les fichiers de vérification. **Le code original de DoModz RGB est conservé dans un dépôt privé.** La compilation ne rend pas un exécutable impossible à analyser.

OpenRGB, Qt, LibreHardwareMonitor et les autres dépendances conservent leurs licences. Les sources tierces requises sont proposées dans l’archive `ThirdParty-Sources-3.1.0.zip`, à côté de l’installateur. Cette archive ne contient pas le code original de DoModz RGB. Consulter [les notices](THIRD-PARTY-NOTICES.md).
