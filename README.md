# node-docker-redis

Start Service
- `sudo docker-compose up --build`
- Visit the following endpoint
    - http://localhost:8080/api/v1/users/Bret
- [Get list of Usernames](https://jsonplaceholder.typicode.com/users)

```sh
docker ps -a # list of all running/stopped/exited containers
docker images -a # list of images
docker volume ls # list of volumes
docker network ls # list of networks
docker network inspect bridge # inepect about bridge network

docker-compose up -d # start container at background
docker-compose down -v # shutdown/remove container with volumes

# check logs to see error, if containers don't work
docker logs redis
docker logs api

docker rmi -f $(docker images -aq) # remove all images if linked to stopped/removed containers
docker system prune -a --volumes # cleanup/remove everything (images, containers, volumes & etc) in one go
```
