  <p align="center">
  <img src="./res/Img/Banner_readme.png" alt="image" width="600" height="auto">
<h1 align="center">LazygitProject</h1>

Bienvenue sur LazygitProject! Il s’agit d’un projet fantastique visant à fournir une solution complète pour notre promo `dev-inté-p2-2024`

## Table des matières

- [Fonctionnalités](#fonctionnalités-mag_right)
  - [Interface Intuitive](#ancre1)
  - [Gestion des Commits](#ancre2)
  - [Gestion des Branches](#ancre3)
  - [Gestion des Stashs](#ancre4)
  - [Gestion des Fichiers](#ancre5)
  - [Rebase Interactif](#ancre6)
  - [ Résolution des Conflits de Fusion](#ancre7)
  - [Visualiseur de Journal](#ancre8)
  - [Personnalisation](#ancre9)
- [Cloner le repositorie](#cloner-le-repositorie-outbox_tray)
- [Installation](#installation-wrench)
  - [Homebrew](#homebrew)
  - [MacPorts](#macports)
  - [Void Linux](#void-linux)
  - [Arch Linux](#arch-linux)
  - [Fedora and RHEL](#fedora-and-rhel)
  - [Ubuntu](#ubuntu)
- [Qu'est-ce que TUI ?](#tui-computer)
- [Cheat sheet](#cheat-sheet-page_with_curl)
  - [Opérations de base](#opérations-de-base)
    - [Stage / Unstage](#ancre10)
    - [Commit](#ancre11) 
    - [Pull / Push](#ancre12)
    - [Navigation](#ancre13)  
    - [Branches](#ancre14) 
  - [Autres fonctionnalités](#autres-fonctionnalités)
    - [Cherry-pick](#ancre15)
    - [Rebase interactif](#ancre16)
    - [Commande personnalisé](#ancre17) 
- [Convention de nommage](#convention-de-nommage-bookmark_tabs)
- [Exercice](#exercice-open_file_folder)
- [Contributing](#contribution-pencil2)
- [FAQ](#faq-books)

##  Fonctionnalités :mag_right:


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

## Cloner le repositorie :outbox_tray:

```
https://github.com/Simplon-hdf/projet-lazygit-roastingmachin.git
```
## Installation :wrench:

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
Pour voir les dernières versions, allez sur [cette page](https://repology.org/project/lazygit/versions).

## TUI :computer:

  <p align="center">
  <img src="./res/Img/TerminalTUI.jpeg" alt="image" width="300" height="auto">

Pour en savoir plus sur le TUI consulter notre fiche [ici](./src/TerminalTUI.md).

## Cheat Sheet :page_with_curl:

  <p align="center">
  <img src="./res/Img/Image_cheatsheet.jpeg" alt="image" width="300" height="auto">

Voici une liste de commandes et d'opérations courantes pour utiliser LazyGit :

### - Commandes principales :

1. **`Space` ou `Enter`** : Sélectionner un fichier pour l'ajouter à la zone de staging ou ouvrir le fichier pour affichage.

2. **`Tab`** : Basculer entre les différentes sections de l'interface (fichiers, staging, commits, etc.).

3. **`c`** : Faire un commit.

4. **`q`** : Quitter LazyGit.

### - Opérations de base :

1. **Stage / Unstage :**<a id="ancre10"></a>
   - Appuyez sur `space` pour ajouter ou retirer un fichier de la zone de staging.
   - Utilisez `space` sur un fichier indexé pour annuler les modifications d'un fichier déjà indexé.

2. **Commit :**<a id="ancre11"></a>
   - Appuyez sur `c` pour ouvrir la fenêtre de commit.
   - Saisissez un message de commit, puis appuyez sur `entrée` pour valider le commit.

3. **Pull / Push :**<a id="ancre12"></a>
   - Appuyez sur `P` pour push.
   - Appuyez sur `p` pour pull.

4. **Navigation :**<a id="ancre13"></a>
   - Utilisez les flèches haut et bas pour naviguer dans la liste des fichiers et les commits.
   - Utilisez les touches `Page Up` et `Page Down` pour naviguer plus rapidement.

5. **Branches :**<a id="ancre14"></a>
   - se rendre dans l'onglet `3`.
   - Appuyez sur `n` pour créer une nouvelle branche.
   - Pour jongler entre les branches utiliser `espace`
   - Pour merge des branches :`M`.

### - Autres fonctionnalités :

1. **Cherry-Pick :**<a id="ancre15"></a>
   - Se rendre and la fenetre `4`
   - Appuyez sur `shift-c` copier le commit selectionée.
   - Appuyez sur `shift-v` pour coller le commit.

2. **Rebase interactif :**<a id="ancre16"></a>
   - Appuyez sur `i` pour ouvrir le menu de rebase interactif.

3. **Commande personalisée :**<a id="ancre17"></a>
   - Appuyez sur `:` pour lancer une commande personalisée.

Utilisez ces raccourcis et commandes pour accélérer votre flux de travail Git avec LazyGit.

Accès a la page [ici](./src/cheatsheet.md).

## Convention de nommage :bookmark_tabs:

<p align="center">
    <img src="./res/Img/Name_Convention.png" width="300" height="auto">
</p>
  
  1. ### Nommage des fichiers :
  - Pas d'espace dans le nom du fichier (utilisation du "**-**" --> kebab-case | ou du "**_**"  --> snake-case pour les espaces)
  - Pas de caractère spécial
  - Les dates sous formats **AAAA-MM-JJ** (année-mois-jour)
  - Le premier élément suivant la date sera l'élément le plus explicite


  2. ### Convention des commits : 
  - Structure du commit : 
    
    <type>[étendu optionnel]:< description>
    [corp optionnel]
    [pied-de-page optionnel] 

  - fix : un type _fix_ répare les bug de code

  - feat : un type _feat_ ajoute une nouvelle fonctionnalité

  - BREAKING CHANGE : un commit avec le pied _BREAKING CHANGE_ : _,_ ou un _!_ après le type, induit une rupture de compatibilité avec l'API (application programming interface ou interface de programmation d'application)

  - Autre commit utilisant la convention Angular :  

 |type|description|
 |----|-----------|
 |build:| Changement qui affecte le build system ou des dépendances externes|
 |ci:| Changement de notre fichier et scripts de configuration CI|
 |docs:| Changement uniquement dans la documentation|
 |perf:| Changement du code afin d'améliorer les performances|
 |refactor:| Un changement de code qui n'ajoute ni des fonctionnalités ni des corrections de bugs |
 |style:| Changement qui n'affecte pas le code|
 |test:| Ajoute ou modifie des tests|
 |chore| Modification de fichier sans affecter le code|

  3. ### Étendue optionnelle :
    - Pointe le fichier spécifique.

  4. ### Commit Description : 
    - Utiliser le **présent**. Utiliser "Add fonctionnalité xy" or "Add tests pour"
    - Cela ne doit pas dépasser plus de **100 characters**.

  5. ###  Pied-de-page optionnel
    - Contient les infos pour le type _Breaking Change_

La page [ici](./docs/Convention.md)

## Exercice :open_file_folder:

  <p align="center">
  <img src="./res/Img/logo exercice.jpeg" alt="image" width="300" height="auto">

Toujours un peu flou pour vous ? rien de telle que de s'exercer pour mieux comprendre. Voici un petit exercice pour vous entrainer et ainsi de mieux comprendre [Lazygit](./docs/exo.md).

## Contribution :pencil2: 

Nous aimons votre participation! Veuillez consulter le [guide de contribution](./src/Contributing.md).

## FAQ :books:

Que représentent les couleurs commit ?
- Vert : le commit est inclus dans la branche master
- Jaune : le commit n’est pas inclus dans la branche master
- Rouge : le commit n’a pas été poussé vers la branche amont

-------------------------
 [retour à la table des matières](#table-des-matières)