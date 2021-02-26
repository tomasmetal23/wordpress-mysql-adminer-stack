# wordpress-mysql-adminer-stack
Docker Stack para un servicio de wordpress independiente.



Fix wordpress cannot load css, js, pictures.

Fixed by adding the following to the very top (after the <?php ) of wp-config.php

if ( (!empty( $_SERVER['HTTP_X_FORWARDED_HOST'])) || (!empty( $_SERVER['HTTP_X_FORWARDED_FOR'])) ) { $_SERVER['HTTPS'] = 'on'; }
