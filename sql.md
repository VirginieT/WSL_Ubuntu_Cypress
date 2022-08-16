https://marketplace.visualstudio.com/items?itemName=cweijan.vscode-mysql-client2

## 1 - Installer MySQL

```
sudo apt update && sudo apt upgrade
sudo apt install mysql-server
mysql --version
sudo service mysql start
sudo mysql -u root -p

```

## 2 - Exemple commandes
https://dev.mysql.com/doc/mysql-getting-started/en/

```
SHOW DATABASES;
CREATE DATABASE <>;
DROP DATABASE <>;
select user, host from mysql.user;

```

## 3 - Version secure (à faire)
https://docs.microsoft.com/fr-fr/windows/wsl/tutorials/wsl-database
```
sudo mysql_secure_installation

```


## 4 - Récap
https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-20-04-fr


