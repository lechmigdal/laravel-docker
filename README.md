# Larvel docker

All what is required for quickly building of docker containers with laravel/composer.

This is a base setup that uses only official images/distributions of php5, apache, laravel and composer. 

# Additional activities to consider

You may want to map the following folders (e.g. using `docker -v`)
- Map the `/var/log/apache2` to an external folder so that docs are stored outside of container
- Map `/var/www/laravel/{app,public,vendor}/` folders for your application specific code
- Map `/etc/ssl` to use custom SSL keys

More information about folders mapping - https://docs.docker.com/engine/tutorials/dockervolumes/

Another option is to customize the Dockerfile and put your SSL keys and application code directly into the container.
