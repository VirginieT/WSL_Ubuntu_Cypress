```
sudo apt-get --purge remove php-common
```

https://devanswers.co/how-to-upgrade-from-php-7-x-to-php-8-on-ubuntu-apache/
Extensions : https://computingforgeeks.com/how-to-install-php-on-ubuntu-linux-system/

```
sudo add-apt-repository ppa:ondrej/php

sudo apt-get update

sudo apt-get install php8.0

sudo service apache2 restart
```


PHP 8 + extensions
```
sudo apt install php8.0-common php8.0-mysql php8.0-xml php8.0-xmlrpc php8.0-curl php8.0-gd 
php8.0-imagick php8.0-cli php8.0-dev php8.0-imap php8.0-mbstring php8.0-opcache php8.0-soap php8.0-zip php8.0-intl -y

sudo service apache2 restart
```


Installing PHP Composer on Ubuntu
https://linuxize.com/post/how-to-install-and-use-composer-on-ubuntu-20-04/
```
sudo apt update

sudo apt install wget php-cli php-zip unzip
```
```
wget -O composer-setup.php https://getcomposer.org/installer

sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
```
When a new Composer version is available, you can update your installation using the following command:
```
sudo composer self-update  
```

Symfony
https://symfony.com/download
```
curl -1sLf 'https://dl.cloudsmith.io/public/symfony/stable/setup.deb.sh' | sudo -E bash

sudo apt install symfony-cli
```

Node
https://docs.microsoft.com/fr-fr/windows/dev-environment/javascript/nodejs-on-wsl
```
sudo apt-get install curl

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

command -v nvm
```
Répertoriez les versions de Node actuellement installées
```
nvm ls
```
Installer la version LTS stable actuelle de Node.js (recommandée pour les applications de production) 
```
nvm install --lts

node --version

npm --version
```
