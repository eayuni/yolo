## Yolo Containerized e-commerce website

### Base Image
node:10:alpine - used this due to the small size, suitable for mongodb

### Docker

#### Client
1. Download the docker image
2. Set the working directory
3. Copy package,json files to the working directory
4. Install dependencies 
5. Copy all files to the current dir
6. Expose port 3000
7. Run the start command

#### Backend
1. Download the docker image
2. Set the working directory
3. Copy package,json files to the working directory
4. Install dependencies 
5. Copy all files to the current dir
6. Expose port 5000
7. Run the start command

#### Database
1. Run the mongo image
2. Set the volume for persistence
3. Set the port to 27017
4. Set the network to allow communication with the other containers


#### Network
Network set to use driver:bridge
Database uses the set network
Backend depends on set database set network
Client depends on backend set network

#### Volume
Volume set for database container, this is for data persistence on addition of product

## Setup/Installation Requirements
Clone repository from github

git clone https://github.com/eayuni/yolo.git

cd yolo

sudo docker-compose build

sudo docker-compose up



