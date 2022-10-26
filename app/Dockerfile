# Define the version of node used
FROM node:16

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY package*.json ./

RUN npm install

# To bundle the app's source code
COPY . .

EXPOSE 8080

CMD [ "node", "index.js" ]

