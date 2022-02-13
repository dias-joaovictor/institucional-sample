# Institucional Sample
### Objetivo
Construir uma projeto institucional sample para implantar no kubernetes. 

### Pré requisitos
* [Docker](https://docs.docker.com/get-docker/)
* [Docker Hub Account](https://hub.docker.com/signup)

<br>

## Comandos
### Construção da imagem docker
```
docker build -t institucionalsample .
```
### Execução da imagem local
```
docker run --name nginx-institucional -d -p 8080:80 institucionalsample
```

### Checar se está executando
```
docker ps
```

### Autenticar no Docker Hub
```
docker login
```

### Push da imagem
```
docker tag institucionalsample:latest <docker hub user>/institucionalsample:latest
docker push <docker hub user>/institucionalsample:latest
```

### Pull da imagem
```
docker pull <docker hub user>/institucionalsample:latest
```

### Execução da imagem do repositório
```
docker run --name nginx-institucional -d -p 8080:80 <docker hub user>/institucionalsample:latest
```

### Execução da imagem do repositório(Meu repositório)
```
docker run --name nginx-institucional -d -p 8080:80 silverfoxjv/institucionalsample:latest
```

### Stop todos os containers rodando
```
docker stop -t0 $(docker ps -aq)
```

### Remover todos os containers
```
docker stop -t0 $(docker ps -aq)
```

<br>

### Créditos
- [Origem do Source](https://www.free-css.com/free-css-templates/page275/hook)

