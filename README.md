# CODTECH-TASK3
DOCKER CONTAINERIZATION

NAME: Shivanshu Tyagi 
COMPANY: Codetech IT Solutions 
ID: : CT4D3182 
DOMAIN: Devops 
DURATION: June to July 2024

#Overview of project: 
Project: DOCKER CONTAINERIZATION
Objective: Containerizing a web application using Docker to ensure consistent environments across development, testing, and production. Writing a Dockerfile to containerize a
simple web application. Build and run Docker containers locally.

Key Activities: Here are the steps how I containerized my web app written in golang.

        1. We write a simple web-application in golang. You can see that in main.go file. The web-app returns Hello World when main file is run and we expose this on port 8080
           so whenever we run the code in local system than, we can access this web-app on browser using localhost:8080
        2. After this for creation of docker image we create a dockerfile in which we defined all the things required to build the image.
        3. After the creation of dockerfile now we need to run some commands in the terminal to make the image of the file
             i.e. to build the code
                                  "docker build -t myapp:latest ."
             once the image is build we can check it using
                                  " docker images"
        4. Now lets create the container from the image we created and than access the web-app
             for creating container run the command
                                  "docker run -d -p80:8080 myapp:latest"
        *here -d is demon mode and -p defines port mapping as pur dockerfile says exposed port is 8080 and docker port is 80 lastly we define image name
                                 "docker ps -a"    // to check all running containers
        5. now go to web browser and type localhost:8080 you can see Hello World page
 
