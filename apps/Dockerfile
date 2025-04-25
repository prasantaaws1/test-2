FROM node:18-alpine

WORKDIR /app
RUN npm i express dotenv
RUN npm i nodemon --save-dev
COPY package*.json ./
RUN npm install
COPY . .

CMD [ "npm", "index.js" ]
