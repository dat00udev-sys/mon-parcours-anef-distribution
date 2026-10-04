# Mon Parcours ANEF — distribution en préparation

Ce dépôt reste privé jusqu'au GO de publication du propriétaire. Application indépendante du ministère de l'Intérieur. Aucun code applicatif, identifiant ANEF, dossier personnel ou clé privée ne doit être ajouté.

## Fichiers préparés

- `versions.json` : enveloppe signée ECDSA P-256/SHA-256 avec la clé de production du propriétaire. Version de référence 0.5.1, code 6 ; aucune restriction ni date de fin. Lien prévu vers la Release v0.5.1.
- `SHA256SUMS.txt` : empreinte de l'APK de validation 0.5.1, à remplacer lors de toute nouvelle compilation.
- Release v0.5.1 : brouillon de validation, pas une version publique finale. L'APK ne contient pas encore la configuration du service de versions.

Le lien vers une Release en brouillon n'est pas disponible pour les téléphones. Aucun token GitHub ne doit être intégré à l'application pour contourner cela.

## Avant diffusion

1. Construire une nouvelle APK release signée avec la même clé Android, avec la configuration publique du manifeste incluse. Utiliser un nouveau versionCode supérieur à 6 et mettre à jour le nom, le tag, les notes, le lien et l'empreinte. Ne pas réutiliser un numéro pour des binaires différents.
2. Tester l'installation de mise à jour et la conservation des données. Ne pas désinstaller l'application officielle de test pour lancer des tests debug.
3. Après GO de publication : rendre le dépôt public, réactiver GitHub Pages (main, racine, HTTPS), publier la Release finale et le manifeste correspondant signé ; vérifier les URL sans connexion GitHub.
4. Tester la chaîne réelle : vérification, bandeau, téléchargement, installation et retour dans l'app. La migration Play reste à valider lorsque sa fiche existe.

Adresse prévue : https://dat00udev-sys.github.io/mon-parcours-anef-distribution/versions.json

Clé publique de vérification dans `versions-public.der` (format DER/X.509, non secrète). Les clés privées restent hors du dépôt.
