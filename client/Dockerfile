
# Pull Docker Hub base image
FROM node:16.14-alpine3.14 
# Set working directory
WORKDIR /usr/app
# Install app dependencies
COPY package*.json ./
RUN npm install -qy --legacy-peer-deps
# Copy app to container
COPY . .
# Run the "dev" script in package.json
CMD ["npm", "run", "start"]