# Docker 

As many people know Docker is a program used to run programs without having them installed in the computer. It uses a new concept known as containerization. This is described as the process to put things into a container and make it run there.

For make the magic happen you need to know a few things(concepts), that may be new if you don't have any experience with something like this. 

The first thing is the base of everything in this platform, container. This is the basic component of any Docker based program. That is said because every program you run in Docker is mounted over one of this structures. 



## Linux like systems

### Container creation



### Downloading images 

//***Proceso para montar una instancia de docker***

Sentencia para crear un contenedor de docker con la imagen de postgres con el nombre de la base de datos y el puerto al que se conecta:
sudo docker run -d --name pepetest  -p 5432:5432 postgres

Sentencia para montar un proyecto sql sobre el puerto de la compu donde se encuentra el contenedor de docker:
sudo psql -h localhost -p 5432 -d postgres -U postgres  < /home/jesus/Escritorio/Proyecto1FULL.sql

Sentencia que muestra los contenedores de docker:
sudo docker ps

Sentencia para ver los puertos y lo que escucha la compu en cada uno de ellos:
sudo lsof -i -P -n | grep LISTEN

Sentencia para ver los contenedores inactivos:
sudo docker ps -a

Sentencia para detener y eliminar un contenedor:
sudo docker container stop [container]
sudo docker container rm [container]

***Aqui termina el proceso***

## Windows

### Creación de un Contenedor 



