# FROM node:19.6

# WORKDIR /app

# COPY package*.json ./
# RUN npm install
# COPY .. ./

# CMD [ "node", "index.js" ]


# Create image based on the official Node image from dockerhub
FROM node:lts-buster
 
# Create app directory
WORKDIR /usr/src/app
 
# Copy dependency definitions
COPY package*.json ./
# COPY package-lock.json ./package-lock.json
 
# Install dependencies
#RUN npm set progress=false \
#    && npm config set depth 0 \
#    && npm i install
RUN npm install
 
# Get all the code needed to run the app
COPY . .
 
# Expose the port the app runs in
EXPOSE 3000
 
# Serve the app
# CMD ["npm", "start"]

CMD [ "node", "index.js" ]
