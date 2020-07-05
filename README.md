# Creating Docker Image for Money Authenticatior App

<table align='left'>
<tr>
<td><img src='https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRGC3QKIepLyjCOgiPl2VS4QTCoUJfrce38nBg0SEAwJw&usqp=CAU&ec=45673586' width='500' /></td>
</tr>
</table>



### Libraries and Tools used in this project

For this activity, we will need a library specialized in deep learning called Keras. We will also use sklearn, a very complete library for machine learning in Python.
<table align='left'>
<tr>
<td><img src='https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSY-TODDr1a7bkYp-J05nq8V3AXl4nb95tKJf6uBqGhhw&usqp=CAU&ec=45673586' width='200' /></td>
    
<td><img src='https://cdn-images-1.medium.com/max/1200/1*00pL0zLnfI7y8d5G1aQrHA.jpeg' width='200' /></td>
    
<td><img src='https://matplotlib.org/_static/logo2.svg' width='200' /></td>
    
<td><img src='https://tse1.mm.bing.net/th?id=OIP.AvJibK-BbuwLDwzedOVIkAHaCl&pid=Api&P=0&w=456&h=160' width='200' /></td>   
    
</tr>
</table>


1) Write Docker File
2) Building the Docker Image
3) Running Money Auteticator APP which was created 

1.a Building the Docker Image
  docker build -t money_api . (Space dot)

See the Dockers

Docker ps

running the dockers ( docker by defalut will run in our docker image)
docker run -p 8000:8000 money_api













1. how to search a docker image in hub.docker.com
```sh
docker search httpd
```
2. Download a docker image from hub.docker.com
```sh
docker image pull <image_name>:<image_version/tag>
```

3. List out docker images from your local system
```sh
docker image ls
```

4. Create/run/start a docker container from image
```sh
docker run -d --name <container_Name> <image_name>:<image_version/tag>

d - run your container in back ground (detached)
```

5. Expose your application to host server
```sh
docker run -d  -p <host_port>:<container_port> --name <container_Name> <image_name>:<Image_version/tag>

docker run -d --name httpd_server -p 8080:80 httpd:2.2
```

6. List out running containers
```sh
docker ps
```

7. List out all docker container (running, stpooed, terminated, etc...)
```sh
docker ps -a
```

8. run a OS based container which interactive mode (nothing but login to container after it is up and running)

```sh
docker run -i -t --name centos_server centos:latest
i - interactive
t - Terminal
```

9. Stop a container 
```sh
docker stop <container_id>
```

10. Start a container which is in stopped or exit state

```sh
docker start <container_id>
```
11. Remove a container

```sh
docker rm <container_id>
```

12. login to a docker container
```sh
docker exec -it <container_Name> /bin/bash
```
