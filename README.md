# Wordpress-nginx-mysql-adminer-stack with traefik as a proxy
Docker Stack for a standalone wordpress service, bitnami image as the basis. 

Deploy
------
First we copy the env-example file to .env, we assign our data to variables.

``` $ git clone https://github.com/tomasmetal23/wordpress-mysql-adminer-stack.git ```

``` $ docker-compose up -d ```

DB & Adminer
------------
mysql server = mysql

database user = root 

You can access from adminer
![Example adminer](https://i.imgur.com/p6YnOnV.png)
