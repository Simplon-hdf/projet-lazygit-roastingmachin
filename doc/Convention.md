# Convention de nommage
  
  1. ## Nommage des dossiers :
  - pas d'espace dans le nom du fichier (utilisation du "**-**" --> kebab case)
  - pas de caractère spécial
  - pas de majuscule (certains language sont sensible à la casse)

  2. ## Licence :

  3. ## Convention de nommage des images :

  4. ## Convention des commit : 
     structure du commit : 
    
    <type>[étendu optionnel]:< description>
    [corps optionnel]
    [pieds optionnel] 


 1. fix : un type _fix_ répare les bug de code

 2. feat : un type _feat_ ajoute une nouvelle fonctionnalité

 3. BREAKING CHANGE : un commit avec le pied _BREAKING CHANGE_ : _,_ ou un _!_ après le type, induit une rupture de compatibilité avec l'API (application programming interface ou interface de programmation d'application)

 4. Autre commit utilisant la convention Angular :  

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

 - ### étendu optionnel :
    * pointe le fichier spécifique.

  - ### Commit Description : 
    * Utiliser le **présent **. Utiliser "Add fonctionnalité xy" or "Add tests pour"
    * Cela ne doit pas dépasser plus de **100 characters**.
    