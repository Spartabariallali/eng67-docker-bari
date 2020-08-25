## Docker Push Commands

### Adding an Docker Image to Dock hub

```
docker images - to find the specific image id

docker tag "add the image ID"

docker tag 4bb46517cac3 bariallali/bari-docker-eng67:Second_commit_adding_nginx_image

docker push bariallali/bari-docker-eng67
```

### How to run the container from a remote repository

```
docker run -d -p 100:3000 aosborne17/getting-started:First_Commit

docker run -d -p 80:80 bariallali/bari-docker-eng67:Second_commit_adding_nginx_image
```

### Docker deleting images

```
docker rmi bariallali/bari-docker-eng67:Second_commit_adding_nginx_image
```


### What is Docker?
- open source software for containerisation - developing, shipping and running applications

- What is the difference between VM and Docker containerisation
- VM emulate a OS and therefore are resource intensive while containerisation shares the machines resources making it super light weight.

### What are the benefits of Docker?
- Consist delivery of your application
- light weight
- open-source
- Can be scaled up significantly using Kubernetes


### Docker client - localhost
- Host machine --> API calls --> Docker Daemon --> Docker Hub

                  Docker pull

                  Docker Push

                  Docker run


Docker looks for containers on the local host first and if they are not available makes an API call that connects with the Docker Daemon. If the image does not exist within the docker daemon it goes to the docker hub and returns the image to the local host.
