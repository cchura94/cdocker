## Comandos Docker
### Para quitar el sudo en el comando (sudo docker) Ubuntu
```
sudo usermod -aG docker $USER
```
### buscar imagenes en Docker hub
```
docker search nom_imagen
docker search postgres
docker search mysql
docker search mariaDB
```
### descargar imagenes de docker hub
```
docker pull nom_imagen
docker pull nom_imagen:tag
docker pull node
docker pull node:18

```
## Imagenes
### lista de imagenes
```
docker image ls
docker images
```
### Eliminar imagenes
```
docker rm (ID_IMAGEN o NAME)
docker image rm d60dc4bd84c0
docker image rm d60
docker rmi d60dc4bd84c0
docker rmi d60
```
### Eliminar imagenes que estan sin uso
```
docker image prune -a
```

## Contenedores
### lista de contenedores
```
docker container ls
docker ps
docker ps -a
```
### Eliminar contenedores
```
docker container rm (ID_IMAGEN o NAME)
docker container rm d60dc4bd84c0
docker container rm d60
docker rm d60dc4bd84c0
docker rm d60
```

### para levantar o correo contenedores

```
docker container run -p 8000:80 nginx
```