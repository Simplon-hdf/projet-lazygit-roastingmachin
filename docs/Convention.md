<p align="center">
    <img src="../res/Img/Name_Convention.png" width="300" height="auto">
</p>

# Convention de nommage
  
  1. ## Nommage des fichiers :
      - Pas d'espace dans le nom du fichier (utilisation du "**-**" --> kebab-case | ou du "**_**"  --> snake-case pour les espaces)
      - Pas de caractère spécial
      - Les dates sous formats **AAAA-MM-JJ** (année-mois-jour)
      - Le premier élément suivant la date sera l'élément le plus explicite


  2. ## Convention des commit : 
     Structure du commit : 
    
    <type>[étendu optionnel]:< description>
    [corp optionnel]
    [pied-de-page optionnel] 

  1. fix : un type _fix_ répare les bug de code

  2. feat : un type _feat_ ajoute une nouvelle fonctionnalité

  3. BREAKING CHANGE : un commit avec le pied _BREAKING CHANGE_ : _,_ ou un _!_ après le type, induit une rupture de compatibilité avec l'API (application programming interface ou interface de programmation d'application)

  4. Autre commit utilisant la convention Angular :  

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

  - ### Étendue optionnelle :
    * Pointe le fichier spécifique.

  - ### Commit Description : 
     * Utiliser le **présent**. Utiliser "Add fonctionnalité xy" or "Add tests pour"
    * Cela ne doit pas dépasser plus de **100 characters**.

  - ###  Pied-de-page optionnel
    * Contient les informations pour le type _Breaking Change_