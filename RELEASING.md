# Publier une release (aide-mémoire)

Ce dépôt est la vitrine publique de pChat : il ne contient pas le code (qui reste dans le dépôt
privé `baptisteftr/pChat`), seulement la présentation, les builds et le flux Sparkle.

Tout passe par `release.sh`, à la racine du dépôt privé :

1. écrire `release-notes/<version>.md` et le commiter : ce qui change pour l'utilisateur, en
   français puis en anglais sous un `---` (modèle : `release-notes/1.0.md`) ;
2. `./release.sh 1.1` (ou `./release.sh` pour ne monter que le build) : archive, signature
   Developer ID, notarisation, `.dmg`, puis release `v<version>` ici avec le `.dmg`, le `.zip`
   et l'`appcast.xml` ;
3. commiter le numéro de build monté par le script, pousser le tag.

Les copies installées lisent
`https://github.com/baptisteftr/pChat-releases/releases/latest/download/appcast.xml` : c'est
donc toujours la **dernière** release publiée qui fait foi. Ne pas la marquer « pre-release ».

Captures : elles viennent du **mode démo** de pChat (équipe et conversations fictives, réglages
par défaut), jamais d'une vraie session — ce dépôt est public. Depuis le dépôt privé :

    xcodebuild -scheme pChat -configuration Debug -derivedDataPath build/DerivedData build
    swift Scripts/demo-shots.swift build/DerivedData/Build/Products/Debug/pChat.app ../pChat-releases/images

Le script produit `chat.png`, `thread.png` et `settings.png`, déjà référencées par le `README.md`.
