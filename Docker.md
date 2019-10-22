# Docker 

As many people know Docker is a program used to run programs without having them installed in the computer. It uses a new concept known as containerization. This is described as the process to put things into a container and make it run there.

For make the magic happen you need to know a few things(concepts), that may be new if you don't have any experience with something like this. 

The first thing is the base of everything in this platform, container. This is the basic component of any Docker based program. That is said because every program you run in Docker is mounted over one of this structures. 



## Linux like systems
This sentence shows all the containers. If it is typed without the *-a* it only shows the containers that are active at the time it's used.
```
sudo docker ps -a
```

The next sentences are used to stop and remove container. These two are recomended to be used together, the main reason is that you can not remove a container that isn't stopped. 
```
sudo docker container stop [container]
sudo docker container rm [container]
```
The next code is used to start a container that has been stopped at some point. 
```
docker start [OPTIONS] CONTAINER [myContainer]
```
The reason is not important here; but if you need some kind of restriction, you can include some of the options included here. If there is no need of any of those you can leave the instruction without them.


### Downloading images 
It is needed to add the corresponding code to make the 

### Creating a container in Docker and using it to mantain a Postgres database
First thing to know is how to create a container in Docker. This particular instruction has the postgres image, database name and the to port it is listening to.
```
sudo docker run -d --name [name]  -p [5432:5432] [postgres]
```

The next code is used to mount an SQL proyect in the port that the container(with postgres) is listening to.
```
sudo psql -h [localhost] -p [5432] -d postgres -U [postgres]  < [dir\file.sql]
```
