## LAMP Stack (Linux, Apache, MySQL(MariaDB), PHP)

[https://www.howtoforge.com/tutorial/install-apache-with-php-and-mysql-on-ubuntu-16-04-lamp/](https://www.howtoforge.com/tutorial/install-apache-with-php-and-mysql-on-ubuntu-16-04-lamp/)

### root

```
sudo su
```

### install maria db

```
apt-get -y install mariadb-server mariadb-client
```

setting secure configuration

```
mysql_secure_installation
```

>Enter current password for root (enter for none): <-- press enter  
Set root password? [Y/n] <-- y  
New password: <-- Enter the new MariaDB root password here  
Re-enter new password: <-- Repeat the password  
Remove anonymous users? [Y/n] <-- y  
Disallow root login remotely? [Y/n] <-- y  
Reload privilege tables now? [Y/n] <-- y  


Test the login

```
mysql -u root -p
```

### Install Apache 2.4

```
apt-get -y install apache2
```
>check `http://ip`  
The document root of the apache default vhost is /var/www/html on Ubuntu and the main configuration file is `/etc/apache2/apache2.conf`. The configuration system is fully documented in `/usr/share/doc/apache2/README.Debian.gz`.

### Install PHP 7

Ubuntu 16.04 이전 버전인 경우

```
add-apt-repository ppa:ondrej/php
apt-get update
```

Ubuntu 16.04 이후 버전부터는 바로 설치.
```
apt-get -y install php libapache2-mod-php
```
