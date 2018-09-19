**Docker project with Nginx php-fpm mysql phpmyadmin**<br>
_start project for local assembly_

`vim /etc/hosts` - put in this file "127.0.1.1 docker-project"<br>
`docker-compose up`<br>
`http://localhost:8080/` - in browser input this and autorization as login: root password: root<br>
`after autorization create table "test" and download dump in table test from dockerProject/autorun/mysql/test.sql`<br>
`http://docker-project:3031/` - in browser input this and see<br>



______________________________________________________________
**WARNING! Commands for remove all docker containers!**
    
*Remove all containers №1*
sudo docker rm $(sudo docker ps -a -q)
*Remove all containers №2*
sudo docker rmi $(sudo docker images -q)   
