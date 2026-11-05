<p align="center"><img src="icon.png" width="128" height="128" alt="Icône de pChat"></p>

<h1 align="center">pChat</h1>

<p align="center"><strong>Un client macOS natif pour kChat, la messagerie d'Infomaniak.</strong></p>

pChat remplace l'app web de kChat par une vraie app Mac : écrite en Swift et SwiftUI, connectée
en temps réel à votre instance kChat, elle reste légère, se pilote au clavier et suit l'apparence
du système.

<!-- Captures : images/*.png, voir RELEASING.md -->

## Télécharger

1. Téléchargez `pChat-x.y.dmg` depuis la [dernière release](../../releases/latest).
2. Ouvrez-le et glissez **pChat** dans le dossier Applications.
3. Au premier lancement, indiquez l'adresse kChat de votre équipe et un **token Infomaniak**
   à scope kChat ; pChat le range dans le Trousseau.

pChat est une app Developer ID notarisée : elle s'ouvre sans avertissement de Gatekeeper. Elle se
**met ensuite à jour toute seule** (Sparkle) : elle cherche une nouvelle version une fois par jour,
ou tout de suite depuis pChat › Rechercher les mises à jour…, et chaque mise à jour est signée et
vérifiée avant d'être installée.

**Configuration requise :** macOS 26 ou plus récent.

Ce dépôt ne contient que les builds publiés, leurs notes de version et le flux de mise à jour.
pChat est en développement actif ; son code source n'est pas publié.

## Fonctionnalités

**Messagerie**
- Messages en **temps réel**, **fils** de discussion, citations, messages épinglés.
- **Réactions** et **emojis personnalisés** du serveur, Markdown complet.
- **Pièces jointes** : images, vidéos et **GIF** (Giphy), aperçus des liens YouTube.
- **Sondages**, et **recherche** dans les messages.

**Organisation**
- Channels publics et privés, conversations **1:1** et de groupe, dans une sidebar réorganisable.
- **Statut** personnalisé, et des **routines** qui le changent selon l'heure.
- Un accès depuis la **barre des menus**, et la fenêtre qui se range au lieu de quitter.

**Intégrations**
- **GitLab** : issues et merge requests à insérer depuis le composeur.

**Confort**
- **Notifications** macOS par channel, avec aperçu masquable.
- **Thèmes** clairs et sombres, éditeur de thème personnalisé.
- **Verrouillage** par Touch ID après une absence.

## Retours

Bugs et idées sont les bienvenus dans les [Issues](../../issues).

## Licence

pChat est un logiciel propriétaire. © 2026 Baptiste Fortier. Tous droits réservés.
Les builds publiés peuvent être téléchargés et utilisés gratuitement. Leur redistribution, ou
l'usage de pChat ou de ses ressources dans un produit commercial, n'est pas autorisé sans accord
écrit. Le code source n'est pas publié dans ce dépôt. pChat n'est ni édité ni soutenu par
Infomaniak.
