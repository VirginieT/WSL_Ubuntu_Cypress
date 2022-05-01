https://docs.microsoft.com/fr-fr/windows/wsl/setup/environment#set-up-your-linux-username-and-password



## 1 - Configurer votre nom d'utilisateur et votre mot de passe Linux


## 2 - Mettre à jour et mettre à niveau des packages

```
sudo apt update && sudo apt upgrade

```



## 3 - Configurer Windows Terminal

https://docs.microsoft.com/fr-FR/windows/terminal/install



## 4 - Stockage Fichier


```
\\wsl$\<DistroName>\home\<UserName>\Project

```


## 5 - Utiliser Visual Studio Code

https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack



## 6 - Configurer la gestion des versions avec Git

https://docs.microsoft.com/fr-fr/windows/wsl/tutorials/wsl-git

Fiche Kourou : chercher "SSH", puis choisir sur "Git et Github"
OU
https://medium.com/featurepreneur/setting-up-ssh-key-with-github-for-ubuntu-cd8f2fabf25b

```
ssh-keygen -t ed25519 -C "votre-email@exemple.fr" 
cat ~/.ssh/id_ed25519.pub

```

Github : Settings > SSH and GPG keys > New SSH key > Coller le contenu de la clé et valider




## 7 - Aliases

```
cd ~
sudo nano .profile
```

Ajouter: 

```
# My Aliases
alias start-pg='sudo service postgresql start'
alias run-pg='sudo -u postgres psql'
```

## 8 - After uninstalling packages from Linux, it’s advised to run these two commands.
```
sudo apt-get autoclean
```

Press Y and ENTER if prompted.
```
sudo apt-get autoremove
```
