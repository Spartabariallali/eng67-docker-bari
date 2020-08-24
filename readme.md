## Docker Push Commands

### Adding an Docker Image to Dock hub

```
docker images - to find the specific image id

docker tag "add the image ID"

docker tag 2e0bee1c6966 bariallali/bari-docker-eng67:second_ commit_pushing_nginx_container

docker push bariallali/bari-docker-eng67
```

### How to run the container from a remote repository

```
docker run -d -p 100:3000 aosborne17/getting-started:First_Commit
```
