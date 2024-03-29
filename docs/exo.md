# <p align='center'>Utilisation de LazyGit 101</p>

<p align='center'>

Pour faire l'exercice, vous aurez besoin d'avoir installé LazyGit. Voici un lien pour [l'installer](../src/Install.md) 

</p>  

- [ ] Les 4 étapes de création d'un repo
   - [ ] Créer le repo GitHub
   - [ ] Cloner le repo GitHub en local
   - [ ] Faire un `git remote -v`
   - [ ] Créer un fichier `toto`
- [ ] écrire sur la ligne 1 du fichier `toto`
- [ ] Lancer LazyGit avec la commande `lazygit`. Vous devriez avoir ceci dans le terminal :
![image](../res/Img/exo/menu-principal.png)
- [ ] Ajouter le fichier que vous venez de créer dans la staging
   - Le sélectionner : on peut naviguer avec les flèches ou en faisant des clics 
   - Utiliser le raccourci `espace` pour l'ajouter 

- [ ] Faire un commit avec comme message `doks: création d'un fichier` (oui la faute est voulue)
   - Le raccourci pour commit est `c`

- [ ] Faire un pull/push (les push et pull sont dirigés de base vers l'origine)
   - Le raccourci pour pull est `p`
   - Le raccourci pour push est `P`

- On va voir maintenant comment renommer un commit
   - [ ] Sélectionner le commit dans l'onglet et utiliser le raccourci `r`
- [ ] creation d'une branch du nom de "testing"
   - `n`dans l'onglet 3
- vous êtes à présent dans la branch testing [ ] creér un fichier peu importe le nom
- modifier la ligne 1 du fichier toto
- [ ]nous allons maintenant merge les 2 branches
   - dans l'onglet 3 `M` sur `testing` en ayant checkout la main avec `espace` 
- pour gérer les conflits utilisés vscode ou pour ceux qui ont installer _Vim_ vous pouvez utiliser le raccourci `e` dans __lazygit__

- [ ]pour ceux qui veulent customisé lazygit on vous propose ce [fichier](../res/exemple-de-config.yml) comme base et si vous voulais ajouter des commande en plus voici le [lien](https://github.com/jesseduffield/lazygit/wiki/Custom-Commands-Compendium#pushing-to-a-specific-remote-repository) pour sa:  
   - les différente commande:
   - `f1` pour faire un pull en choisisant la branche et le remote
   - `f2` pour choisire le remote pour push
   - `ctrl-v`pour faire un commit conventionelle 
   