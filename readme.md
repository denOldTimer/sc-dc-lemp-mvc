
![image](https://github.com/denOldTimer/sc-dc-lemp/blob/master/docker-lemp.jpg)


# Docker-compose LEMP stack
 
## nginx - php - mysql - node

nginx
  - nginx:stable-alpine
  - container name : scnginx
  - ports: "9080:80"

php
  - php:8.0-fpm
  - container name : scphp
  - ports: "9000:9000"

mysql
  - mysql:8.0.30
  - container name: scdb
  - ports: "9306:3306

node
  - node:latest
  - container name: scnode   





---

### TESTING YOUR DOCKER COMPOSE CONTAINERS
```js
    sudo docker compose logs scnginx
```

---


### IN CASE OF ERROR FROM THE DATABASE.
To test connection I use   **_dBeaver_**   to connect.   
Remeber to change the port number.   
   
```js
    Public Key Retrieval is not allowed
```

I got the following error that was simple to fix [check out the link](https://ganeshchandrasekaran.com/dbeaver-public-key-retrieval-is-not-allowed-77eba055bbcd)

---

### TODO
- Create a general config folder 
- create a cheetsheet of all the commands one needs to know but can't remember, lol



