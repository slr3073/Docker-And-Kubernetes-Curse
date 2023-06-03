FROM node

# Par defaut le working dir est la racine et les commandes (voir RUN npm install) sont exécutés dans le working dir
WORKDIR /app

# Le dossier /app sera créé sur le conteneur s'il n'existe pas
COPY . /app

# Sera executé à la création de l'image
RUN npm install

# Ne fait rien, juste de la documentation : le port est configuré au lancement du conteneur
EXPOSE 80

# Sera executé lors du lancement d'un conteneur
CMD ["node", "server.js"]


# Lorsque le l'on construit le conteneur les changements sont détectés :
#  si un couche change toutes les couches suivantes sont re-executé normalement.
# Les couches sans changements sont quant à elles simplement cachés