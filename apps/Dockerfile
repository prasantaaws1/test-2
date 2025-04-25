FROM node:19.6

WORKDIR /app
RUN npm install
COPY package*.json ./

COPY .. ./
CMD [ "node", "index.js" ]
