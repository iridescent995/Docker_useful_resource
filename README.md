# Docker_useful_resource
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
### Docker remove all volumes 
```
docker volume prune
```
### Docker find container name from image name 
```
docker ps --format '{{.Image}}' | grep "<image name>"
```
### Docker find container id from container name 
```
docker ps -aqf "name=<container name>"
```
### Docker form image from a container 
```
docker commit <container name> <new image name>
```
