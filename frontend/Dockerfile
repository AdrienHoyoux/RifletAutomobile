# Dockerfile pour le développement avec hot reload
FROM node:18-alpine

# Répertoire de travail dans le conteneur
WORKDIR /app

# Copier package.json et installer les dépendances
COPY package*.json ./
RUN npm install

# Copier le reste des fichiers de l'application
COPY . .

# Exposer le port du serveur de développement Vue.js (par défaut 8080)
EXPOSE 8080

# Commande pour démarrer le serveur de développement Vue.js avec hot reload
CMD ["npm", "run", "serve"]
