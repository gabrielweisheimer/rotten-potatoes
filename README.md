### Aula 2 - Questão 4 ###
- Passos para deploy da aplicação no kubernetes:

# Build da Imagem
1) docker build -t gweisheimer/rotten-potatoes:v1 -f /etc/git/rotten-potatoes/Dockerfile src/

2) docker push gweisheimer/rotten-potatoes:v1

3) docker tag gweisheimer/rotten-potatoes:v1 gweisheimer/rotten-potatoes:latest

4) docker push gweisheimer/rotten-potatoes:latest

# Deploy da aplicação
1) kubectl apply -f k8s/deployment.yaml


# rotten-potatoes

## Configuração

MONGODB_DB => Nome do database

MONGODB_HOST => Host do MongoDB

MONGODB_PORT => Posta de acesso ao MongoDB

MONGODB_USERNAME => Usuário do MongoDB

MONGODB_PASSWORD => Senha do MongoDB
