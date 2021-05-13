## INSTALACE Linux 
* ano
* ČR
* ano
* hlubucekserver
* hlubucek
* hlubucek
* hlubucek
* ne
* ano 
* Asistované - použít celý disk a nastavit LVM 
* "zvolíš disk" 
* ano
* pokračovat
* ano 
* HTTP proxy NE -> pokračovat 
* Instalovat bezpečnostní aktualizace automaticky 
* zvolíme -> DNS, LAMP, Samba, standard system utilities, OpenSSH root -> root 
* ano 
* "dokončit instalaci" 
 
 
## ROOT 
* sudo passwd root
* sudo root 

## UPDATE SYSTEMU  
* apt-get update
* apt-get install mc 
 
 
## DATABAZE 
* mysql -u root -p 
 
* CREATE DATABASE wordpress; 
* CREATE USER hlubucek IDENTIFIED BY "hlubucek"; 
* GRANT ALL PRIVILEGES ON wordpressdb.* TO hlubucek; 
* FLUSH PRIVILEGES; 
* EXIT 
 
 
## INSTALACE WORDPRESS 
* cd /tmp 
* wget http://wordpress.org/latest.zip 
* unzip -q latest.zip -d /var/www/html/ 
* chown -R www-data:www-data /var/www/html/wordpress 
* chmod -R 755 /var/www/html/wordpress 
* mkdir -p /var/www/html/wordpress/wp-content/uploads 
* chown -R www-data:www-data /var/www/html/wordpress/wp-content/uploads 	 
 
 
## NA OBOU VIRTUALECH NASTAVÍME VNITŘNÍ SÍŤ (Linux i Win10) 
 
* ifconfig -> zjistíme ip 
 
* -> win10 prohližeč -> ip linuxu/wordpress 
 
* cz 
* pokracovat 

* wordpress    (nazev databaze z linuxu)
* root         (uživatel)
* root         (heslo)
* "ip linux serveru" 
* wp_           
 
* TestWeb      (nazev webu)
* admin        (uživatel)
* "admin"      (heslo)
* admin@jeto.jedno 
 
* přihlásit se 
 
 
 ### Video: https://www.youtube.com/watch?v=oLsA2kj_bMU 
