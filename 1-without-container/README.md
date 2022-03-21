1. git clone https://github.com/manjitsingh-yadav/docker-session.git 
2. cd 1-without-container
3. git checkout master

4. php -f src/index.php -S 0.0.0.0:8080
5. curl localhost:8080/src/index.php
6. curl localhost:8080/src/index.php -I
