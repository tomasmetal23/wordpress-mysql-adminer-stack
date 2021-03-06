# Wordpress-nginx-mysql-adminer-stack with traefik as a proxy
Docker Stack para un servicio de wordpress independiente, bitnami nginx wordpress como base.

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
