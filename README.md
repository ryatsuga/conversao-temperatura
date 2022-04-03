# Studying Docker and Kubernetes

Dockerfile container image montage;
Kubernetes local deploy with Deployment and Service.

## Getting started

### Docker

1. Acessar diretório "src" pelo prompt de comando;
2. Rodar o comando: "docker image build -t <seu-username>/conversao-temperatura:v1 ." para gerar a imagem do container;
3. Rodar o comando "docker container run -dp 8080:8080 <seu-username>/conversao-temperatura:v1" para rodar o container;
4. Acessar o web app rodando localmente em: localhost:8080

### Kubernetes

1. Criar um cluster:
   - k3d: "k3d cluster create --agents 3 --servers 3 -p "8080:30000@loadbalancer"
2. Acessar diretório "src/k3s" pelo prompt de comando;
3. Rodar o comando "kubectl apply -f deployment.yaml" e aguardar criação dos elementos (pods, replicasets, services...);
4. Acessar o web app rodando localmente em: localhost:8080
