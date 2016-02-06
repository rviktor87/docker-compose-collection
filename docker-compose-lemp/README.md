#Consists of
 - php:fpm
 - mysql:latest
 - nginx:latest

#Some specification
Nginx and php uses /var/www/html directory by default, so I wouldn't like to mess with it.
Therefore in the nginx container the host's `./public/` will mapped to `/var/www/html/`, and the `default.conf` changed to use this path.
In the php container the host's `./` will mapped to `/var/www/html/`, so PHP can access to other directories than `public`.
