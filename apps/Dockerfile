FROM node:19.6

WORKDIR /app
RUN apk update && apk add npm
COPY package*.json ./
RUN npm install
COPY .. ./
CMD [ "node", "index.js" ]
