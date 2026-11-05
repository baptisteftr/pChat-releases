# Publier une release (aide-mémoire)

Ce dépôt est la vitrine publique de pChat : il ne contient pas le code (qui reste dans le dépôt
privé `baptisteftr/pChat`), seulement la présentation, les builds et le flux Sparkle.

Tout passe par `release.sh`, à la racine du dépôt privé :

1. écrire `release-notes/<version>.md` (ce qui a changé, en français) ;
2. `./release.sh 1.1` (ou `./release.sh` pour ne monter que le build) : archive, signature
   Developer ID, notarisation, `.dmg`, puis release `v<version>` ici avec le `.dmg`, le `.zip`
   et l'`appcast.xml` ;
3. commiter le numéro de build monté par le script, pousser le tag.

Les copies installées lisent
`https://github.com/baptisteftr/pChat-releases/releases/latest/download/appcast.xml` : c'est
donc toujours la **dernière** release publiée qui fait foi. Ne pas la marquer « pre-release ».

Captures : les mettre dans `images/` et les référencer dans le `README.md`. **Vérifier qu'aucun
message, nom ou channel réel n'y apparaît** : ce dépôt est public.
