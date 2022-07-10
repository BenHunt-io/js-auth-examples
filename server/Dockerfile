FROM node:16

# Create app directory inside container
WORKDIR /app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install

# Bundle app source
COPY . .

# What port that docker will expose
EXPOSE 8080

# Finally, the runtime of the application docker is hosting
CMD [ "node", "server.js" ]