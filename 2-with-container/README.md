1. git clone https://github.com/manjitsingh-yadav/docker-session.git 
2. cd 2-with-container
3. git checkout master

4. docker build -f Dockerfile -t phpinfo:2022-03 .
5. docker container run --entrypoint php -v $PWD/src/:/src/:ro -w /src/ --name phpinfo phpinfo:2022-03 -f index.php -S 0.0.0.0:8080 
6. docker logs phpinfo 
7. docker exec phpinfo wget http://localhost:8080 --spider -S -q
