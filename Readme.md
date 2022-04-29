# Build da Imagem
1) docker build -t gweisheimer/rotten-potatoes:v1 -f ./Dockerfile src/

2) docker push gweisheimer/rotten-potatoes:v1

3) docker tag gweisheimer/rotten-potatoes:v1 gweisheimer/rotten-potatoes:latest

4) docker push gweisheimer/rotten-potatoes:latest

# Subir com um comando:

docker-compose up -d