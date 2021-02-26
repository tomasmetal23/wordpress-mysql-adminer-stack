# Wordpress-mysql-adminer-stack with traefik as a proxy
Docker Stack para un servicio de wordpress independiente.

Deploy
------
First we copy the env-example file to .env, we assign our data to variables.

$ docker-compose up -d

DB & Adminer
------------
mysql server = mysql

database user = root 

You can access from adminer
![Example adminer](https://i.imgur.com/p6YnOnV.png)

Fix wordpress cannot load css, js, pictures
--------------------------------------------

Fixed by adding the following to the very top (after the <?php ) of wp-config.php

if ( (!empty( $_SERVER['HTTP_X_FORWARDED_HOST'])) || (!empty( $_SERVER['HTTP_X_FORWARDED_FOR'])) ) { $_SERVER['HTTPS'] = 'on'; }
