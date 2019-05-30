# simple-docker-php-apache

Build the image from the Dockerfile and tag it as `simple-docker-php-apache`:

```sh
docker build -t simple-docker-php-apache .
```

Run the built image as a container with a bind mount:
```sh
docker run -d -p 8080:80 -v "$(pwd)"/php:/var/www/html/ simple-docker-php-apache
```
