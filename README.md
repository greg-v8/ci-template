# Continuous Integration Template
This repo is to serve as a template for a continuous integration solution that uses the following technologies:
- Git/GitHub
- Travis CI
- Docker Hub
- Amazon AWS

### Steps for a local Docker Hub build:
1. download the latest version of Docker Hub
2. clone this repo and `cd` into it
3. create a new dev machine: `docker-machine create -d virtualbox dev`
4. tell Docker to talk to the dev machine: `eval "$(docker-machine env dev)"`
5. build and run a container for the hello-world app: `docker-compose up`
6. get the ip of the dev machine: `docker-machine ip dev`
7. open a browser and navigate to the ip from step 6

### Coming soon...
- Travis CI integration
- Docker Hub Automated Build
- Amazon AWS integration
