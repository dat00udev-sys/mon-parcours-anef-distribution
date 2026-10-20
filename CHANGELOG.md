# Nouveautés

## 1.1.0 — 20 octobre 2026

- **Synchronisation plus rapide et qui ne reste plus bloquée** :
  - les lectures ANEF se font en parallèle ;
  - chaque actualisation est limitée à 45 secondes ;
  - le détail des nouveaux messages est lu après l’affichage du résultat ;
  - une rubrique qui ne répond jamais n’est plus retentée.
- **L’étape en cours s’affiche** (« Lecture de votre dossier… »). Un second appui pendant une actualisation est signalé, au lieu d’être ignoré.
- **Message clair après chaque actualisation** : « 2 nouveautés : … » ou « Rien de nouveau depuis la dernière actualisation ». Si ANEF répond trop lentement, l’appli le dit.
- **Accueil simplifié** : une ligne discrète pour l’état de l’actualisation, le bloc « Depuis votre dernière visite » (ancien statut → nouveau statut), la carte du dossier, « À faire », et une seule carte quand une action est nécessaire.
- **Réglages réorganisés** : une page d’accueil avec cinq catégories (compte, suivi et notifications, apparence et langue, sécurité et données, mises à jour). Chacune ouvre sa propre page.
- **Notifications de statut** : elles indiquent le nouveau statut et l’ancien.

Version Android : code **11**, identifiant **fr.monparcours.anef**. Android 10 et suivants. Même signature que les versions précédentes. La 1.0.0 et la 1.0.1 restent prises en charge : installez la 1.1.0 par-dessus quand l’appli vous le propose.

Tests : 67 tests unitaires et 24 tests Android sans échec, dont un tour complet des écrans et des pages de réglages en français, anglais et arabe.

## 1.0.1 — 14 octobre 2026

- Plus fluide : les données chiffrées sont lues une seule fois par écran, au lieu de l’être à chaque affichage ou pour chaque message.
- Notifications plus claires : les catégories portent leur nom dans les réglages d’Android, et un rappel affiché en mode discret dit « Vous avez un rappel ».
- Confirmation après la suppression de données, message quand il n’y a aucun rappel, et retour visible quand on active ou coupe le suivi automatique ou le verrouillage.
- Outils de compilation et bibliothèques mis à jour (Android Gradle Plugin 9.4, Compose 1.12, jsoup 1.23). L’appli se comporte exactement comme avant et pèse un peu moins.

Version Android : code **10**, identifiant **fr.monparcours.anef**. Android 10 et suivants. Même signature que les versions précédentes. La 1.0.0 reste prise en charge : installez la 1.0.1 par-dessus quand l’appli vous le propose.

Tests : 61 tests unitaires et 23 tests Android sans échec, dont un tour complet des écrans en français, anglais et arabe.

## 1.0.0 — 7 octobre 2026

Première version stable, après un audit de sécurité complet.

- **Mise à jour obligatoire** : les versions 0.5.3 et antérieures ne sont plus prises en charge. Elles affichent « Version plus prise en charge » et n’actualisent plus les données ANEF. Installez la 1.0.0 par-dessus, sans désinstaller : vos données sont conservées.
- Identifiant et mot de passe : le clavier ne les mémorise plus et ne les corrige plus.
- Protection contre les applis qui recouvrent l’écran pendant la connexion et la suppression de données (Android 10 et 11).
- Numéros de dossier copiés marqués comme sensibles : absents de l’aperçu du presse-papiers et de l’historique du clavier.
- Documents PDF déchiffrés uniquement en mémoire pendant la lecture (Android 11 et suivants).
- Widget discret par défaut : le statut ne s’affiche que si vous l’activez dans les réglages.
- Aperçu des applis récentes masqué quand le verrouillage de l’app est activé (Android 13 et suivants).
- Messages d’erreur toujours compréhensibles, sans texte technique.
- Un ancien fichier de versions ne peut plus masquer une version plus récente.

Version Android : code **9**, identifiant **fr.monparcours.anef**. Android 10 et suivants. Même signature que les versions précédentes.

Tests : 58 tests unitaires et 18 tests Android sans échec. Tests de sécurité sur émulateur : écrans internes inaccessibles aux autres applis, données illisibles hors de l’app, application non débogable.

## 0.5.3 — 4 octobre 2026

- Liens longs du profil mieux affichés, sans premières lettres rognées.
- Nom du document dans le titre du lecteur PDF.
- Icônes d’heure et d’aide corrigées ; textes des états vides simplifiés.
- Affichage de la version et textes améliorés en arabe.
- Version de développement séparée de l’application officielle ; variante de démonstration retirée.
- Vérification des mises à jour configurée, avec manifeste signé et liens limités au dépôt de distribution.

Version Android : code **8**, identifiant **fr.monparcours.anef**. Android 10 et suivants.

APK vérifiée : signature Android de production identique aux versions précédentes. Les rapports locaux recensent 56 tests unitaires sans échec. Les 17 tests Android et la mise à jour 0.5.2 → 0.5.3 sans perte des données sont documentés par Claude. Certains avertissements lint ont des exceptions documentées.

À valider au lancement : chaîne réelle de mise à jour via GitHub public. À compléter : téléphone réel, Android 10, TalkBack, relecture arabe et migration Play.
