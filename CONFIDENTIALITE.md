# Confidentialité

Document de présentation du fonctionnement de la version 0.5.3, mis à jour le 4 octobre 2026.

## Sur le téléphone

Les données récupérées depuis ANEF et les documents téléchargés sont conservés localement. Les secrets et données du coffre sont protégés par chiffrement avec Android Keystore. L’enregistrement des identifiants est optionnel. Les sauvegardes cloud et transferts Android de l’application sont désactivés.

Il n’existe pas de serveur Mon Parcours conservant vos identifiants ou dossiers, ni de publicité intégrée. Les données locales ne sont pas ajoutées au dépôt GitHub.

## Connexions externes

- **ANEF et son service de connexion** reçoivent les requêtes nécessaires pour vous authentifier et consulter votre compte.
- **GitHub** héberge la distribution et le fichier signé de versions. Les requêtes peuvent exposer l’adresse IP et le nom/version du client, sans transmettre les identifiants ou le contenu du dossier ANEF.
- Les fonctions du **Journal officiel** et les liens de documentation consultent les publications et sites externes concernés. Ces sites appliquent leurs propres règles.

La confidentialité locale ne signifie donc pas que l’app fonctionne sans échanges réseau.

## Vos choix

Vous pouvez choisir l’enregistrement des identifiants, le suivi automatique, les alertes, la visibilité des détails dans les notifications, le verrouillage et les captures. Les captures sont bloquées par défaut ; la connexion ANEF reste protégée.

La suppression locale se fait depuis les réglages, avec choix des catégories et confirmation. Désinstaller l’app supprime ses données locales ; elle ne supprime pas votre dossier ANEF. Il n’existe pas de sauvegarde cloud Mon Parcours permettant de restaurer ces données.

## Signalement d’un problème

Ne publiez jamais un mot de passe, code de connexion, numéro de dossier, document ou capture personnelle dans les issues. Décrivez le problème avec la version de l’application, Android et les étapes de reproduction. Ce dépôt de distribution n’est pas un canal pour transmettre des dossiers administratifs.
