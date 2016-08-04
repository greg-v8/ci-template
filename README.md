# Continuous Integration Template
This repo is to serve as a template for a continuous integration solution that uses the following technologies:
- Git/GitHub
- Travis CI
- Docker Hub
- Amazon AWS

### Steps for a local Docker Hub build:
1. download the latest version of Docker Hub
2. clone this repo and `cd` into the `app` directory
3. create a new Docker host: `docker-machine create -d virtualbox dev`
4. tell Docker to talk to the new host: `eval $(docker-machine env dev)`
5. build and run a container for the hello-world.js app: `docker-compose up`
6. open a new terminal and get the ip of the dev machine: `docker-machine ip dev`
7. open a browser and navigate to port 3000 of the ip from step 6

### Important Commands
Remember to check your env when using a new terminal:
`docker-machine env <docker-machine name>`

Open a docker container to see your app:
`docker exec -i -t <container id> /bin/bash`

### Coming soon...
- Travis CI integration
- Docker Hub Automated Build
- Amazon AWS integration
