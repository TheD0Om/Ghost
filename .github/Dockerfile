# Utilise l'image officielle Node.js comme image de base
FROM node:14

# Définis le répertoire de travail dans le conteneur
WORKDIR /usr/src/app

# Copie les fichiers de définition de dépendances dans le répertoire de travail
COPY package*.json ./

# Installe les dépendances
RUN npm install

# Copie les fichiers et dossiers du projet dans le répertoire de travail du conteneur
COPY . .

# Expose le port sur lequel l'application va tourner
EXPOSE 2368

# Commande pour démarrer l'application
CMD [ "npm", "start" ]
