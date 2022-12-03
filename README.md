Aprés avoir crée mon cv avec html et css, j'ai configuré le fichier dockerfile:
FROM nginx:alpine
COPY . /usr/share/nginx/html : je lui donne le chemin vers lequel le cv sera coipé.

j'ouvre le terminal et j'exécute la commande : 
docker build -t webserver-image:v1  pour créer une image sur docker

docker run -d -p 80:80 webserver-image:v1
