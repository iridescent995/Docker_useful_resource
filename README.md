# Docker cheat sheet
All docker useful Commands and resource


### Docker start with logs 
```
docker start -ai container_name
```
### Docker stop all containers 
```
docker stop $(docker ps -aq)
```
### Docker rm all containers
```
docker rm $(docker ps -aq)
```
### Docker remove all unused volumes 
```
docker volume prune
```
### Docker remove all images
```
docker rmi -f $(docker images -aq)
```
### Docker find container name from image name 
```
docker ps --format '{{.Image}}' | grep "<image name>"
```
### Docker find container id from container name 
```
docker ps -aqf "name=<container name>"
```
### Docker form an image from a container 
```
docker commit <container name> <new image name>
```
### Docker rename image 
```
docker tag <old image name> <new image name>
```
