### Docker project with nginx, php-fpm, mysql and phpmyadmin
_start project for local assembly_

Append this line to /etc/hosts:

    127.0.1.1 docker-project

Start docker with command:

    docker-compose up
    
Open this url with browser:

    http://localhost:8080/

and autorize using login: root, password: root.

After autorization create table "test" and download dump in table test from dockerProject/autorun/mysql/test.sql

Paste this address into your browser and see:

    http://docker-project:3031/


______________________________________________________________
**WARNING! Commands to remove all docker containers!**
    
*Remove all containers*

    sudo docker rm $(sudo docker ps -a -q)

*Remove all images*

    sudo docker rmi $(sudo docker images -q)

