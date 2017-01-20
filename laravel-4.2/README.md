
# running

    docker build -t laravel-4.2 .
    docker run -p 8000:80 -d -v $PWD/simple-laravel/:/var/www/html laravel-4.2

# Get a shell on a running container

    docker ps  # get container id
    docker exec -it <container-id> /bin/bash

# TODO
* setup appropriate DocumentRoot and other Apache configuration
