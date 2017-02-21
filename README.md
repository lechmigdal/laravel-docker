# Larvel docker

All what is required for quickly building of docker containers with laravel/composer.

Using only standard images for php5 +  apache + laravel + composer base setup. 

# Additional activities to consider

You may want to (e.g. using `docker -v`)
- Map the `/var/log/apache2` to an external folder so that docs are stored outside of container
- Map `/var/www/laravel/{app,public,vendor}/` folders for your application specific code
- Map `/etc/ssl` to use custom SSL keys

More information about folders mapping - https://docs.docker.com/engine/tutorials/dockervolumes/

Another option is to customize the Dockerfile and put your SSL keys and application code directly into the container.
