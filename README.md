Dockerfile source: https://github.com/RaffaeleDAlessandro/Url-Shortener/tree/master/Dockerfile-master

Installation guide

Remember to set port 8080 into Virtual-Box

Start boot2docker or docker-machine

$ boot2docker start
$ boot2docker ssh
Clone this repository

$ git clone https://github.com/GruppoPBDMNG-1/Dockerfile.git
Building of image

$ docker build --tag=gruppo_pbdmng_1/urlshortener Dockerfile
Create and run the container

$ docker run -d --name urlshortener -p 8080:8080 gruppo_pbdmng_1/urlshortener
Enter into container

$ docker exec -it urlshortener bash
Launch the application

$ ./start
To see the application in action open this link: http://localhost:8080 in your web broswer.
