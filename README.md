# docker-wordpress-demo
# How to build the docker with the Dockerfile in this repo?
* Download this repo 
* Navigate inside the repo directory 
* run the following command 

```
docker build -t <tag> .
```
Example:
```
docker build -t iwordpress-app . 
```

# How to run this image ?
```
docker run -p <nodeport>:<containerport> -d <conatiner-name>
```
Example:
```
docker run -p 80:80 -d cwordpress-app 
```

# How to push this local image to dockerhub?

## Tag your image
```
docker tag <localimage>:<tag> <dockerhub-username>/<remoteimage>:<tag>
```

Example:
```
docker tag wordpress:php7.1-apache javeedsocial/iwordpress-app:v1.0
```

##Push the image to remote repo on dockerhub 
```
docker push <dockerhub-username>/<remoteimage>:<tag>
```
Example
```
docker push javeedsocial/iwordpress-app:v1.0
```
