# Projeto Kubernetes: Integração ChatGpt.

## Criando Cluster
```
    k3d cluster create meucluster --servers 3 --agents 3 -p "3000:30000@loadbalancer" -p "8080:30001@loadbalancer"
```