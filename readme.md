**Docker project with Nginx php-fpm mysql phpmyadmin**
**start project**
_for local assembly_

`vim /etc/hosts` - put in this file "127.0.1.1 docker-project"
`docker-compose up`
`http://localhost:8080/` - in browser input this and autorization as login: root password: root
`after autorization create table "test" and download dump in table test from dockerProject/autorun/mysql/test.sql`
`http://docker-project:3031/` - in browser input this and see



**WARNING! Commands for remove all docker containers!**
    
# Remove all containers №1
sudo docker rm $(sudo docker ps -a -q)
# Remove all containers №2
sudo docker rmi $(sudo docker images -q)   