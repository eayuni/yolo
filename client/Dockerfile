FROM node:10-alpine

#setting the working dir to client
WORKDIR /client

#copy pacakage.json file to workdir
COPY pacakage*.json /client/

#install dependencies
RUN npm install

#expose the port to be accessed outside the container
EXPOSE 3000

#run the app
CMD [ "npm" "start" ]



