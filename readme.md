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
