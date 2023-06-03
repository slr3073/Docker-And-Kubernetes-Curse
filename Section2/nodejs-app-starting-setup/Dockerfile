FROM node

WORKDIR /app

# Ici on a fait un optimisation pour éviter de refaire npm install à chaque modification de l'application
COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

CMD ["node", "server.js"]


