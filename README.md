### Nginx MySQL PHP-FPM Docker environment

A very basic docker nginx PHP-FPM and mysql development environment with sane defaults.

phpMyAdmin has been added as a quality of life feature -  http://phpmyadmin.localhost.
See nginx/default.conf for details or to disable or delete from docker-compose to remove.

See http://localhost/info.php for PHP and ZEND details

> [!NOTE]
> * Credentials moved to .env file
> * Amend Dockerfiles and docker-compose files to suit

> [!WARNING]
> * Internal dev network use only
> * There is no SSL. That's kind of an end user thing to sort out with own certs
