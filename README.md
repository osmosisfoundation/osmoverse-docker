# phmxverse-docker

to build a container, navigate to the folder, and run docker build, and specify a name

At the top level, build a phmxversecore image

```
docker build -t "dpastoor/phmxversecore" .
```

This image is used for the mrgsolve images, which overwrites the mrgsolve version 

```
docker build -t "metrumresearchgroup/mrgsolve:v0.7.10" .
```

### remove all stopped containers

 docker rm $(docker ps -qa)

### remove dangling images

docker rmi $(docker images -f dangling=true -q)


### restart a stopped containers

`docker start <containerID>`


### stop all containers

`docker stop $(docker ps -a -q)`
