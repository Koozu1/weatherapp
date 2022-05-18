FROM node:17

#Create app directory
WORKDIR /usr/src/frontend

#Copy package.json and package-lock.json
COPY package*.json ./

RUN npm install

#Bundle sources
COPY . .

#expose port 8080
EXPOSE 8080

CMD [ "node", "server.js" ]