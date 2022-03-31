# Studying Docker

Dockerfile container image montage.

## Getting started

1. Acessar diretório src pelo prompt de comando;
2. Rodar o comando: "docker image build -t <seu-username>/conversao-temperatura:v1 ." para gerar a imagem do container;
3. Rodar o comando "docker container run -dp 8080:8080 <seu-username>/conversao-temperatura:v1" para rodar o container;
4. Acessar o web app rodando localmente em: localhost:8080
