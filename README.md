# This repository will have the summary of whatever I learn from the playlist name "Docker Crash Course Tutorial" from "The Net Ninja"

# Lesson-01 - What is Docker
# We need a specific environment to run a specific project. Sometimes we need to share our project with other developers as well and they need to setup the specific environment to run that particular project. To make this process more efficient, docker comes up with a solution called docker container. In a container, we can put all the things to create a specific environment, and share the container with the other developers as well. In this way, the other developers do not have to spend ample amount of time setting up the environment. The only need to have docker to manage that container. 

# Lesson-02 - Installing Docker
# 1. Install Docker Desktop on Windows (Link: https://docs.docker.com/desktop/install/windows-install/)
# 2. Install Linux on Windows with WSL (Link: https://docs.microsoft.com/en-us/windows/wsl/install)
# 3. Manual installation steps for older versions of WSL (Link: https://docs.microsoft.com/en-us/windows/wsl/install-manual)

# Lesson-03 - Images and Containers
# A. Images
# 1. Images are like blueprints for containers
# 2. Contains Runtime Environment
# 3. Contains Runtime Environment
# 4. Contains Application Code
# 5. Contains Any Dependencies
# 6. Contains Extra Configuration (e.g. env variables)
# 7. Contains Commands
# 8. We cannot change Images, we need to create a new Image in case of we want to change something

# B. Containers
# 1. When we run an Image, it creates a container which run the instaces of an image and also run our application
# 2. Container is an isolated process
# 3. We can share the image to others so that they can run the image which creates the container in their local decices to run the application.

# Lesson-04 - Parent Images and Docker Hub
# A. Docker Images
# 1. Images are made of several layers
# 2. Order of the layers matter
# 3. Typically starts with parent Image: includes the OS and sometimes the runtime environment
# 4. The next layer could be copying the source codes and the dependencies
 
 # B. Docker Hub
 # A. We can pull relevant docker images from the docker hub.

 # Lesson-05 - Dockerfile
# set of instruction to docker to create the image


# Lesson-08 - Layer Chaching
# docker build -t myapp .

# Lesson -09 - Managing Docker

# docker image delete using command

# docker image rm myapp4
# docker image rm myapp4 -f

# docker container delete using command
# docker container rm app_c1

# remove all images and container
# docker system prune -a

# build images including version
# docker build -t myapp:v1 .

# run conatiner using that specific version
# docker run --name myapp_c -p 4000:4000 myapp:v1
