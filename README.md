# Microservices of a streaming platform

<p>
The microservices project for a streaming platform tries to simulate a microservices architecture, it has three microservices: list services, song services and video services. Each of these microservices has independent functions such as:

- **List the songs:** get a list in Json format of the songs with their attributes.

- **Playing the audio of songs:** allows you to listen to only the audio of the songs that exist.

- **Song videos:** allows you to play the video of the existing songs.

It should be noted that this is just a microservices project.
Dockerfile and Docker-compose are also used to create Docker images.
Git Actions automates the creation of images, uploading them to Docker Hub and then deploying them to EC2.
</p>

### How to install and run the project? :wrench:
Node.js technologies are used with the Express.js framework, as well as Dockerfile, Docker-compose and AWS EC2.
The project must first be downloaded or cloned:
- `git clone https://github.com/cdto17/MicroservicesPlatform.git`

The following steps are to install dependencies and run the project:
- `npm init -y`
- `npm install express`
- `npm start`

Steps to build Docker-compose:
- `docker-compose build`
- `docker-compose up`

Command to shut down the container:
- `docker-compose down`

### How to use the project  :white_check_mark:
<p>
To use the project you must execute the commands described in the previous point. When, you run it in the terminal you will be able to find URLs that you can open locally and you will be able to see the different services it offered such as listing the songs, audio and video songs.
</p>

![Docker1](https://github.com/cdto17/MicroservicesPlatform/assets/91480354/5b708f3b-99e8-4611-8662-638c08580059)
![Docker2](https://github.com/cdto17/MicroservicesPlatform/assets/91480354/1b3805c5-9301-4f6e-8f45-5cf6977e69d7)
![Docker3](https://github.com/cdto17/MicroservicesPlatform/assets/91480354/99b62822-001f-4f63-b6f2-b41cd4e5d5fc)
![Docker4](https://github.com/cdto17/MicroservicesPlatform/assets/91480354/743b1331-cc2a-40ce-bf30-d0b2220a847e)

In the screenshots you can see how it works, to see more videos and songs you can change the URL number. 
For example for the video microservice:

http:localhost:8084/api/video/1/play

http:localhost:8083/api/song/1/play

http:localhost:8084/api/video/2/play

http:localhost:8083/api/song/2/play

###  Collaborators :boy:
William Javier Quilumba Imacana
https://github.com/JaviQuilumba

###  License :page_facing_up:
This project is licensed under the (AFL-3.0) License - see the [LICENSE](https://opensource.org/license/afl-3-0-php) file for details.

