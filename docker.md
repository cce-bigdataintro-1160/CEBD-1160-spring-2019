
# Intro 2 Containerization & Shipping Software

### Agenda
* Homework Check
* Learning Conteinerization with Docker
* Homework

### Learning Conteinerization with Docker

##### Goals
Understand the benefits of conteinerizing processes and how to apply it using Docker:

##### Introducing conteinerization
1. Check your `docker version`
2. Check your `docker info`
3. List all possible commands you can do with the docker client.
4. List your currently running containers, check for stopped ones too.
5. Create your first container! Run the official `hello-world` Docker Image. 
6. Read the text that shows up specially the 4 bullet points.
7. List your currently running containers again, check for stopped ones too.
8. Make sure to remove your stopped container.
9. Now start another `hello-world` container using the `--rm` flag. Do you need to remove it after?

##### Images VS Containers
1. List all the images you have downloaded to your local machine.
2. List all the containers you have running or stopped on your local machine.
3. Start a new detached container for 

##### Running Existing Images as Containers
1. Open your browser and type localhost:80 in the url. Now try to reach localhost:8080.
2. Run the following two images at the same time using the same terminal:
* nginx (map the port 80 from the container)
* httpd (map the port 8080:80  from the container)
3. Test the fact your webservers are up by checking the same urls again. You should get a different page for each.
4. Make sure to stop and remove your containers.

##### Getting inside the Container

##### Reflections about Containers
1. Navigate through the [Docker Hub](https://hub.docker.com/) and the [Official Images](https://hub.docker.com/search/?q=&type=image&image_filter=official)
2. Identify two Linux Images: Debian and Ubuntu. 
3. Run an interactive container for each of them and test the curl command on both by using:
   ```apt-get install curl```
   ```curl --version```
   ```curl http://www.concordia.ca/```

##### Modifying existing Images
Customize your own version of : XXX

##### Creating your own Images

##### Final
create the python docker build that will run your projects!
create a docker container that generates fake news!
dockerize an app (run and top an clean) single shot and long running


### Homework
* Don't forget to fill up the Weekly Journal! 

##### Basic

##### Advanced
  
##### Reach

### Optional homework
* What commands we learned are useful for data exploration and why?

### Recommended Readings
* [Getting Started with Docker](https://docs.docker.com/get-started/)
* [Docker Hub](https://hub.docker.com/)


### Advanced exercises material
* Can you complete these challenges from [cmdchallenge](https://cmdchallenge.com/)
