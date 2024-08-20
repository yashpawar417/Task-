# BRAINSTORMFORCE_TASK

Commands
1. Updating the package list

> **sudo apt update**

2. PHP, MySQL and Nginx installation

> **sudo apt install php-fpm php-mysql mysql-server nginx unzip**

3. Configuring Nginx to work with PHP

> **cd /etc/nginx/sites-available**

> **sudo rm default**

> **sudo nano default**

4. Restarting Nginx

> **sudo systemctl restart nginx.service**

5. Removing the default index.html page

> **cd /var/www/html**

> **sudo rm index.nginx-debian.html**

6. Downloading Wordpress to the Ubuntu server

> **sudo wget https://wordpress.org/latest.zip**

7. Extracting the contents of the Wordpress archive

> **sudo unzip latest.zip**

8. Moving WordPress to the server's root folder

> sudo mv wordpress/* .

9. Changing the owner of the Wordpress files

> sudo chown -R www-data:www-data *

10. Securing MySQL installation

> sudo mysql_secure_installation

11. Creating the database and a database user

> sudo mysql

> CREATE DATABASE wordpress_db;

> CREATE USER 'wordpress_user'@'localhost' IDENTIFIED BY 'P@55word';

> GRANT ALL PRIVILEGES ON wordpress_db.* TO 'wordpress_user'@'localhost';

> EXIT;

12. Creating wp-config.php

> sudo nano wp-config.php


