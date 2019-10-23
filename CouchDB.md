# CouchDB

Description of the database

## Install process of CouchDB

Step by step process to install CouchDB in linux

## First Run in CouchDB

To go in the database and make changes as the ones descripted below, it's needed to enter to it as an administrator or someone who has acces to the database. That is made by using the following command in the terminal, replacing [admin] for the user you created when installed the database in your computer.
```
$ HOST="http://[admin]:[admin]@[127.0.0.1:5984]"
$ curl -X PUT $HOST/database
```
That sets the user to be the one you put into the brackets and the ip, port to be the ones after the '@' symbol.
After that is spected from the computer to send an 
```
{"ok":true}
```
Meaning the log in is complete. 

### Creating a database in CouchDB

### Deleting a database in CouchDB

### Creating a design document in CouchDB

### Updating a design document in CouchDB

### Deleting a design document in CouchDB




Taken from: https://guide.couchdb.org/draft/security.html
