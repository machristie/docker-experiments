
Based on https://hub.docker.com/_/php/

Run with

    docker run -P -d --name simple-php-app simple-php

Use `docker ps` to find the port number.

Then go to http://localhost:PORT/test.php

Or, run it in such a way that it maps a local port for the docker port

    docker run -p 8000:80 -d --name simple-php-app simple-php

Now go to http://localhost:8000/test.php

To clean up the container run the following

    docker stop simple-php-app
    docker rm simple-php-app