# Use a old node version
FROM node:10-alpine

# Set the working dir of the container
WORKDIR /usr/src/weatherapp_backend

#copy package and package-lock files
COPY package*.json ./

# Install packages
RUN npm install

# Copy to working dir
COPY . .

#Expose the port 9000
EXPOSE 9000

CMD [ "npm", "start" ]