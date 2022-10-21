# Docker

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la création d'une image docker ✔️
- l'éxécution d'un container ✔️
- l'orchestration de containers avec docker-compose ✔️


## 💻 J'utilise

### Un exemple personnel commenté ✔️

--------------------------------------------------------------------------
#### Dockerfile (client)
--------------------------------------------------------------------------
FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app
COPY package*.json ./
RUN npm i
COPY public public
COPY src src

CMD npm start

-------------------------------------------------------------------------
#### Dockerfile (server)
-------------------------------------------------------------------------
FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app
COPY package*.json ./
RUN npm i
COPY src src

CMD npm start

### Utilisation dans un projet ✔️

[[lien github](https://github.com/MarysaR/docker3)](...)

Description :
- Créer un fichier Dockerfile qui assemble les instructions permettant de compiler une image de l'application.
- Compiler une image Docker
- Démarrer un conteneur à partir de l'image, il est exécuté de façon complétement indépendante du système hôte.
- Partager l'application grâce au DockerHub via Docker Desktop
- Démarrer un serveur (express) dans un conteneur lié à un conteneur (Mongo)
- Exposer un port : pour accéder à une application sur un port particulier il faut spécifier que l'on veut l'exposer sur un port de la machine hôte.
- Se connecter un conteneur distant (Mongo), le démarrer, et via la cmd --link, lier les conteneurs l'un à l'autre (mongo et express-docker)
- Orchestrer plusieurs conteneurs
- Écrire un fichier docker-compose.yml pour l’environnement de développement
- Connecter un volume

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
