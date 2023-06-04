FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

# Apparament pas une bonne pratique car pas de bénéfice mais des problèmes (ex. volumes anonymes) 
# priviligier le paramétrage par lors du lancement (qui est déjà obligatoire btw) 
# VOLUME [ "/app/feedback" ]

CMD [ "npm", "start" ]