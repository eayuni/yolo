FROM node:10-alpine

#set the working directory
WORKDIR /backend

#copy package.json to the working dir
COPY package*.json /backend/

#install dependencies
RUN npm install

#make the port available outside the container
EXPOSE 5000

#run the app at start
CMD [ "npm" "start" ]
