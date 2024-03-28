  <p align="center">
  <img src="./res/Img/User_Manual.png" alt="image" width="300" height="auto">
<h1 align="center">LazygitProject</h1>

Bienvenue sur LazygitProject! Il s’agit d’un projet fantastique visant à fournir une solution complète pour notre promo `dev-inté-p2-2024`

## Table des matières

- [Fonctionnalités](#fonctionnalités)
  - [Interface Intuitive](#ancre1)
  - [Gestion des Commits](#ancre2)
  - [Gestion des Branches](#ancre3)
  - [Gestion des Stashs](#ancre4)
  - [Gestion des Fichiers](#ancre5)
  - [Rebase Interactif](#ancre6)
  - [ Résolution des Conflits de Fusion](#ancre7)
  - [Visualiseur de Journal](#ancre8)
  - [Personnalisation](#ancre9)
- [Cloner le repositorie](#cloner-le-repositorie)
- [Installation](./src/Install.md)
  - [Homebrew](#homebrew)
  - [MacPorts](#macports)
  - [Void Linux](#void-linux)
  - [Arch Linux](#arch-linux)
  - [Fedora and RHEL](#fedora-and-rhel)
  - [Ubuntu](#ubuntu)
- [Qu'est-ce que TUI ?](#terminal-tui-computer)
- [Cheat sheet](./src/cheatsheet.md)
- [Convention de nommage](./docs/Convention.md)
- [Exercice](./docs/exo.md)
- [Contribution](./src/Contributing.md)

##  Fonctionnalités


Lazygit est une interface utilisateur basée sur terminal (TUI) pour Git, conçue pour simplifier et rationaliser les tâches courantes de Git grâce à une interface facile à utiliser. Elle offre une représentation visuelle de l'état du dépôt Git et permet aux utilisateurs d'interagir avec Git sans avoir besoin de se souvenir des options de ligne de commande complexes. Certaines des fonctionnalités remarquables de Lazygit comprennent :

**Interface Intuitive:**<a id="ancre1"></a> Lazygit fournit une interface interactive simplifiée qui affiche l'état actuel du dépôt Git de manière visuellement attrayante.

**Gestion des Commits:**<a id="ancre2"></a>  Les utilisateurs peuvent mettre en scène, retirer de la scène et modifier les changements avec facilité. Lazygit permet aux utilisateurs d'écrire des messages de commit, de sélectionner les fichiers à commiter et de visualiser les différences des changements avant de commiter.

**- Gestion des Branches:**<a id="ancre3"></a> Il permet aux utilisateurs de créer, supprimer, fusionner et basculer entre les branches sans effort. Les utilisateurs peuvent visualiser la structure des branches et gérer les branches via l'interface TUI.

**- Gestion des Stashs:**<a id="ancre4"></a>  Lazygit facilite la gestion des stashes, permettant aux utilisateurs de mettre en stash des changements, de voir les éléments mis en stash, d'appliquer des stashes et de supprimer des stashes selon les besoins.

**- Gestion des Fichiers:**<a id="ancre5"></a>  Les utilisateurs peuvent voir l'état des fichiers individuels, mettre en scène ou retirer de la scène des fichiers et supprimer des changements directement depuis l'interface Lazygit.

**- Rebase Interactif:**<a id="ancre6"></a>  Lazygit prend en charge le rebase interactif, permettant aux utilisateurs de réorganiser facilement les commits, de fusionner plusieurs commits en un seul, de modifier les messages de commit et d'effectuer d'autres opérations pendant le processus de rebase.

**- Résolution des Conflits de Fusion:**<a id="ancre7"></a>  Il fournit une interface simple pour résoudre les conflits de fusion, permettant aux utilisateurs de voir les fichiers en conflit, de choisir entre différentes versions et de résoudre les conflits directement dans l'interface TUI.

**- Visualiseur de Journal:**<a id="ancre8"></a>  Lazygit inclut un visualiseur de journal intégré qui permet aux utilisateurs de naviguer dans l'historique des commits, de voir les détails des commits et d'effectuer des actions telles que le cherry-picking et l'annulation des commits.

**- Personnalisation:**<a id="ancre9"></a>  Les utilisateurs peuvent personnaliser les raccourcis clavier, les couleurs et d'autres paramètres pour adapter l'expérience Lazygit à leurs préférences.

En somme, Lazygit vise à rendre les opérations Git plus accessibles et plus efficaces pour les utilisateurs novices et expérimentés en fournissant une interface visuelle pratique pour les tâches Git courantes.

## Cloner le repositorie:

```
https://github.com/Simplon-hdf/projet-lazygit-roastingmachin.git
```
## Installation

<p align="center">
<img src="./res/Img/installationlogo.png" alt="image" width="300" height="auto">

### Homebrew

Normalement, la formule lazygit peut être trouvée dans le noyau Homebrew, mais nous vous suggérons d’utiliser notre formule pour obtenir celle fréquemment mise à jour. Il fonctionne aussi avec Linux.

Tape:
```
brew install jesseduffield/lazygit/lazygit
```
Core:
```
brew install lazygit
```
### MacPorts

Dernière version construite à partir des versions de github. Tapez :
```
sudo port install lazygit
```
### Void Linux

Les paquets pour Void Linux sont disponibles dans le dépôt de distribution

Ils suivent les dernières versions en amont:
```
sudo xbps-install -S lazygit
```

### Arch Linux

Les paquets pour Arch Linux sont disponibles via pacman et AUR (Arch User Repository).

Il y a deux paquets. Le stable qui est construit avec la dernière version et la version git qui construit à partir du commit le plus récent.

Stable: `sudo pacman -S lazygit`

### Fedora and RHEL

Les paquets pour Fedora/RHEL et CentOS Stream sont disponibles via Copr (Cool Other Package Repo).
```
sudo dnf copr enable atim/lazygit -y
sudo dnf install lazygit
```

### Ubuntu

```
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | grep -Po '"tag_name": "v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/latest/download/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit /usr/local/bin
```

Vérifiez l'installation correcte de LazyGit en exécutant simplement la commande:
```
lazygit --version
```
Une autre méthode existe [ici](./src/Install.md).

## Terminal TUI :computer:

  <p align="center">
  <img src="./res/Img/TerminalTUI.jpeg" alt="image" width="300" height="auto">

Un environnement en mode texte (`TUI`, de l'anglais « Text User Interface », « Textual User Interface » ou encore «Terminal User Interface ») est un rétronyme introduit dans le jargon informatique après l'invention des environnements graphiques pour se distinguer des interfaces en ligne de commande. Ce type d'interface utilisateur occupe la totalité de l'écran comme les interfaces graphiques, et n'est donc pas limité au traitement ligne par ligne comme les `CLI`.

Ce type d'environnement s'avère très utile pour le développement d'applications sans besoins graphiques.

De nombreuses bibliothèques logicielles permettent le développement de telles interfaces utilisateur, sur différentes plates-formes.

Notre fiche [ici](./src/TerminalTUI.md).

## Cheat Sheet

## Convention de nommage



