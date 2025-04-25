FROM node:19.6

WORKDIR /app

COPY package*.json ./

COPY .. ./
RUN npm install
CMD [ "node", "index.js" ]
