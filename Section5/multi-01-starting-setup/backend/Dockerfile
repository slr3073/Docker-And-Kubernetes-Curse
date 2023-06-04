FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV DB_USERNAME=root
ENV DB_PASSWORD=secret

CMD [ "npm", "start" ]