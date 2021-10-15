# docker-wordpress-demo
# How to build the docker with the Dockerfile in this repo?
* Download this repo 
* Navigate inside the repo directory 
* run the following command 

```
docker build -t <tag> .
ex:
docker build -t iwordpress-app . 
```

# How to run this image ?
```
docker run -p <nodeport>:<containerport> -d <conatiner-name>
ex:
docker run -p 80:80 -d cwordpress-app 
```

# How to push this local image to dockerhub?

## Tag your image
```
docker tag <localimage>:<tag> <dockerhub-username>:<tag>

ex:
docker tag wordpress:php7.1-apache javeedsocial/iwordpress-app:v1.0
```
