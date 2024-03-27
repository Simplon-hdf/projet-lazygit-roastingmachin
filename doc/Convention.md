# Convention de nommage
  
  1. ## nommage des dossiers :
    - pas d'espace dans le nom du fichier (utilisation du "**-**" --> kebab case)
    - pas de caractère spécial
    - pas de majuscule (certains language sont sensible à la casse)

  2. ## licence :

  3. ## Convention de nommage des images :

  4. ## Convention des commit : 
     structure du commit : 
    
    <type>[étendu optionnel]:< description>
    <!--------ligne d'espace blanche------------>
    [corps optionnel]
    <!--------ligne d'espace blanche------->
    [pieds optionnel] 


 1. fix : un type _fix_ répare les bug de code

 2. feat : un type _feat_ ajoute une nouvelle fonctionnalité

 3. BREAKING CHANGE : un commit avec le pied _BREAKING CHANGE_ : _,_ ou un _!_ après le type, induit une rupture de compatibilité avec l'API (application programming interface ou interface de programmation d'application)

 4. Autre commit utilisant la convention Angular :  

 |type|description|
 |----|-----------|
 |build:| changement qui affecte|
 |ci:| changes to CI configuration file and scripts|
 |docs:|Documentation changes only|
 |perf:|code change that improve performance|
 |refactor:|a code change that neither fixes bug neither add features|
 |style:| change that not affect the meaning of the code|
 |test:| add or correcting test|
 |chore|modif file without modify the code|

 - ### optional scope :
    * points to a specific component which is affected by the change.

  - ### Commit Description : 
    * Use the **imperative present tense**. Use "Add feature xy" or "Add tests for"
    * It should be no more than **100 characters**long.
    