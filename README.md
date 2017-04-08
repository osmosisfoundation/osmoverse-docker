# osmoverse-docker

## ** WARNING: Docs are very much a work in progress **

All images can be considered alpha-stage and the overall structure will likely be
heavily refactored for maintainability.


## Getting started

to build a container, navigate to the folder, and run docker build, and specify a name

At the top level, build a osmoverse image

```
docker build -t "osmoverse/phmxcore" .
```


## versioning

A given container can be built and versioned for testing or stability purposes. 
For example, to use the mrgsolve-versioned container to build off mrgsolve v0.7.10,
use the v7.1.0 image, with the a command like the following:

```
docker build -t "metrumresearchgroup/mrgsolve:v0.7.10" .
```


# General Docker help


### remove all stopped containers

`docker rm $(docker ps -qa)`

### remove dangling images

`docker rmi $(docker images -f dangling=true -q)`


### restart a stopped containers

`docker start <containerID>`


### stop all containers

`docker stop $(docker ps -a -q)`
