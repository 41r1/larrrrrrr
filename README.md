## php install

* sudo apt update && sudo apt upgrade 
* sudo apt install software-properties-common ca-certificates lsb-release apt-transport-https 
* sudo LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php 
* sudo apt update
* sudo apt install php8.1 
* sudo apt install php8.1 php8.1-fpm php8.1-cli php8.1-curl php8.1-zip php8.1-mysql php8.1-mbstring php8.1-xml php8.1-bcmath
* php -v 

## node install

* curl -s https://deb.nodesource.com/setup_16.x | sudo bash
* sudo apt install nodejs -y
* node -v

## composer 
* sudo apt update
* sudo apt install wget php-cli php-zip unzip
* php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
* HASH="$(wget -q -O - https://composer.github.io/installer.sig)"
* php -r "if (hash_file('SHA384', 'composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
* sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
* composer
///////////
* composer create-project laravel/laravel example-app
* composer global require laravel/installer
* laravel new example-app
* cd example-app
* php artisan serve
