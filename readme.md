# Projeto Kubernetes: Integração ChatGpt.

## Criando Cluster
```
k3d cluster create meucluster --servers 3 --agents 3 -p "3000:30000@loadbalancer" -p "8080:30001@loadbalancer"
```

## Clonar projetos
```
git clone https://github.com/KubeDev/idc-ms-chatgpt.git
```

## Criar imagem chatservice
```
docker build -t usuarioDockerHub/imersao-chatservice:v1 .
```
## Logar no docker hub
```
docker login
```
## Subir imagem chatservice para o docker hub
```
docker push usuarioDockerHub/imersao-chatservice:v1
``` 

## Gerar versão latest da imagem imersao-chatservice
docker tag 4lexandremoreira/imersao-chatservice:v1 4lexandremoreira/imersao-chatservice:latest
## Subir imagem chatservice para o docker hub
```
docker push usuarioDockerHub/imersao-chatservice:v1

```

