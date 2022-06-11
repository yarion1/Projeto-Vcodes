# Dockerfile para Node Express Backend 

FROM node:16.14-alpine3.14 
#here we're defining the working directory
WORKDIR /user/src/api

#copying our dependencies to the container
COPY ./package.json ./
COPY ./package-lock.json ./

#installing all the dependencies that we copied 
RUN npm install


#copying all the files inside the container
COPY . .

#exposing the port so we can access it further
EXPOSE 5000

#starting the server
CMD ["node", "server.js"]