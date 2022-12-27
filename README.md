# LampSetup
For Docker and Virtual Machines even local runtime enviroment that need php backend

  apt update && apt upgrade -y && apt install openssh iproute2 tor -y && sshd <br>      

  sudo su <br>
  apt update <br>
  apt upgrade -y <br>
  apt install sqlite3 apache2 php phpunit php-gd php-sqlite3 php-bcmath php-redis php-gmp  php-interbase php-odbc php-mysql php-curl mariadb-server openssh-server composer git nodejs npm nano neovim vim lynx php-zip -y <br> 
 a2enmod rewrite <br>
 systemctl restart apache2
  
nano /etc/apache2/ports.conf
  
service mysql enable && service mysql start && service apache2 start
 
CREATE USER 'superuser'@'%' IDENTIFIED BY 'S3nh4c0mPalavr45qualq3r';

GRANT ALL PRIVILEGES ON *.* TO 'superuser'@'%' WITH GRANT OPTION;
FLUSH PRIVILEGES;
EXIT;

SET PASSWORD FOR 'root'@'localhost' = PASSWORD('');

# Docker Templates

 
 
touch Dockerfile <br>
FROM debian <br>
RUN apt update <br>
RUN apt upgrade -y <br>
RUN apt install sqlite3 apache2 php phpunit php-gd php-sqlite3 php-bcmath php-redis php-gmp php-interbase php-odbc php-mysql php-curl mariadb-server composer git nodejs npm php-zip -y
RUN a2enmod rewrite <br>
RUN command <br>
LABEL manteiner 'Tester'

