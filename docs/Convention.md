## Convention de nommage

<p align="center">
    <img src="../res/Img/Name_Convention.png" width="300" height="auto">
</p>
  
  1. ### Nommage des fichiers :
  - Pas d'espace dans le nom du fichier (utilisation du "**-**" --> kebab-case | ou du "**_**"  --> snake-case pour les espaces)
  - Pas de caractère spécial
  - Les dates sous formats **AAAA-MM-JJ** (année-mois-jour)
  - Le premier élément suivant la date sera l'élément le plus explicite


  2. ### Convention des commit : 
  - structure du commit : 
    
    <type>[étendu optionnel]:< description>
    [corp optionnel]
    [pied-de-page optionnel] 

  - fix : un type _fix_ répare les bug de code

  - feat : un type _feat_ ajoute une nouvelle fonctionnalité

  - BREAKING CHANGE : un commit avec le pied _BREAKING CHANGE_ : _,_ ou un _!_ après le type, induit une rupture de compatibilité avec l'API (application programming interface ou interface de programmation d'application)

  - Autre commit utilisant la convention Angular :  

 |type|description|
 |----|-----------|
 |build:| changement qui affecte le build system ou des dépendances externes|
 |ci:| changement de notre fichier et scripts de configuration CI|
 |docs:|changement uniquement dans la documentation|
 |perf:|changement du code afin d'améliorer les performances|
 |refactor:|un changement de code qui n'ajoute ni des fonctionnalités ni des corrections de bugs |
 |style:| changement qui n'affecte pas le code|
 |test:| ajoute ou midifie des test|
 |chore|modification de fichier sans affecter le code|

  3. ### étendu optionnel :
    - pointe le fichier spécifique.

  4. ### Commit Description : 
    - Utiliser le **présent**. Utiliser "Add fonctionnalité xy" or "Add tests pour"
    - Cela ne doit pas dépasser plus de **100 characters**.

  5. ###  Pied-de-page optionnel
    - Contient les infos pour le type _Breaking Change_

