#Docker Stack Web Application
###A web stack with docker based apache, php, mysql and maildev

##For begin

- First ! Open the file docker-compose.yml and custom the link volume for the container web and the container mariadb
- You need to specify your folder with your workspace as well as the folder that will contain the files in your database
- And... that's all ;-)!

##Build image php7

- From the command line, go to the folder containing the docker-compose.yml and then do a docker-compose build

##Launch this stack

- Two possibility : run the docker-composer up -d command or start the docker-compose shell that contains the docker-compose -d and the following line: socat TCP-LISTEN:2375,reuseaddr,fork,bind=localhost UNIX-CONNECT:/var/run/docker.sock that opens the docker API for use in an IDE like phpstorm
