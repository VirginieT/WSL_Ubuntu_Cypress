https://docs.microsoft.com/fr-fr/windows/wsl/setup/environment#set-up-your-linux-username-and-password



## 1 - Configurer votre nom d'utilisateur et votre mot de passe Linux


## 2 - Mettre à jour et mettre à niveau des packages

```sudo
`sudo apt update && sudo apt upgrade`

```



## 3 - Configurer Windows Terminal

https://docs.microsoft.com/fr-FR/windows/terminal/install



## 4 - Stockage Fichier


```
`\\wsl$\<DistroName>\home\<UserName>\Project`

```


## 5 - Utiliser Visual Studio Code

https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack



## 6 - Configurer la gestion des versions avec Git

https://docs.microsoft.com/fr-fr/windows/wsl/tutorials/wsl-git

Fiche Kourou : chercher "SSH", puis choisir sur "Git et Github"

```
`ssh-keygen -t ed25519 -C "votre-email@exemple.fr" 
cat ~/.ssh/id_ed25519.pub

```

Github : Settings > SSH and GPG keys > New SSH key > Coller le contenu de la clé et valider




## 7 - Configurer une base de données

https://docs.microsoft.com/fr-fr/windows/wsl/tutorials/wsl-database


### Installer MySQL

```
`sudo apt update
sudo apt install mysql-server
mysql --version
```

```
`sudo /etc/init.d/mysql start
sudo mysql_secure_installation

```

Commandes MySql

```
`sudo mysql
SHOW DATABASES;
CREATE DATABASE database_name;
DROP DATABASE database_name;
```

https://dev.mysql.com/doc/mysql-getting-started/en/

https://marketplace.visualstudio.com/items?itemName=cweijan.vscode-mysql-client2


## 8 - Aliases

```
cd ~
sudo nano .profile
```

Ajouter: 

```
`# My Aliases
alias start-pg='sudo service postgresql start'
alias run-pg='sudo -u postgres psql'
```
