# Installer Mon Parcours

## Avant de commencer

Téléphone Android 10 ou version suivante, connexion Internet pour le téléchargement et la première synchronisation, compte ANEF pour consulter vos demandes. Aucun compte propre à Mon Parcours n’est nécessaire.

Le téléchargement est public et ne nécessite aucun compte GitHub. Ouvrez la [Release 1.0.0](https://github.com/dat00udev-sys/mon-parcours-anef-distribution/releases/tag/v1.0.0) pour retrouver l’APK signée et son empreinte.

## Première installation

1. Ouvrez [Releases](https://github.com/dat00udev-sys/mon-parcours-anef-distribution/releases) et la version **1.0.0**.
2. Dans **Assets**, téléchargez **MonParcours-1.0.0.apk**. Les archives « Source code » ne sont pas l’application.
3. Ouvrez le fichier téléchargé. Si Android le demande, autorisez temporairement l’installation d’applications depuis ce navigateur ou gestionnaire de fichiers. Le nom et l’emplacement du réglage varient selon le téléphone.
4. Confirmez l’installation avec Android, puis ouvrez **Mon parcours**. Vous pouvez retirer ensuite l’autorisation d’installation à cette source.
5. Choisissez votre langue et connectez votre compte ANEF. L’enregistrement des identifiants est facultatif.

## Mettre à jour sans perdre vos données

Téléchargez l’APK plus récente depuis la même distribution et installez-la par-dessus la version existante. Gardez la même application installée. Les mises à jour officielles utilisent la même signature Android.

L’application « Mon parcours (dev) » est réservée aux tests ; elle est distincte et ne doit pas être distribuée aux utilisateurs.

## Vérifier le fichier

Le fichier `SHA256SUMS.txt` contient l’empreinte de l’APK. Pour les utilisateurs qui souhaitent la contrôler sous PowerShell :

```powershell
Get-FileHash .\MonParcours-1.0.0.apk -Algorithm SHA256
```

Empreinte attendue : `3022b15da0ebca919acaf5f22343e6fb687db9c9b422006590100c706efa324c`.

Une empreinte sert à comparer le fichier ; elle ne remplace pas la signature Android ni la confiance dans la provenance du téléchargement.
