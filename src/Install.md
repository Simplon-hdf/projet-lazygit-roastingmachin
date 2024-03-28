  <p align="center">
  <img src="../img/logo-install.png" alt="image" width="300" height="auto">
<h1 align="center">LazygitProject</h1>

# Installation :bookmark_tabs:

1 - Ouvrez le terminal.
2 - Téléchargez le dernier paquet binaire de lazygit avec la commande suivante (remplacez `VER` par la version actuelle) :
```
export VER="0.40.2" && wget -O lazygit.tgz https://github.com/jesseduffield/lazygit/releases/download/v${VER}/lazygit_${VER}_Linux_x86_64.tar.gz
```

3 -Extrayez le fichier téléchargé :
```
tar xvf lazygit.tgz
```
4 - Déplacez le binaire dans un répertoire de votre $PATH, par exemple /usr/local/bin :
```
sudo mv lazygit /usr/local/bin/
```
5 - Vérifiez que l’installation a réussi en exécutant :
```
lazygit -v
```
Cela devrait installer `lazygit` sans avoir besoin d’ajouter un PPA. Assurez-vous de remplacer `VER` par la dernière version disponible sur la page des releases de lazygit.