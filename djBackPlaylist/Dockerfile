# Utilisez l'image officielle de Node.js basée sur Alpine
FROM node:14-alpine

# Définir le répertoire de travail à l'intérieur du conteneur
WORKDIR /usr/src/server

# Copier package.json et package-lock.json dans le répertoire de travail
COPY package*.json ./

# Installer les dépendances du projet
RUN npm install

# Copier le reste du code de l'application dans le répertoire de travail
COPY . .

# Exposer le port sur lequel l'application va tourner
EXPOSE 3001

# Commande pour exécuter l'application
CMD ["npm", "start"]