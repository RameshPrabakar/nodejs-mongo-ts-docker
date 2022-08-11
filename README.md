# CURD Reactjs Application 
This project is simple CURD application using ReactJS, NodeJS, MongoDB and Docker

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)


## General info
Here is an example of a simple tasks application that creates, retrieves, edits, and deletes tasks. We actually run the API on the NodeJS server and you can use MongoDB to save all these tasks.
	
## Technologies
Project is created with:
* Node version: 16.15.0
* NPM version: 8.16.0
* ReactJS version: 17.0.2
* Typescript version: 4.5.5	
* Docker version: 20.10.17

## Service-Mongo-Communication

* Since the MongoDB service name is localhost, the connection string below should be used.
```
MONGO_CONNECTION_STRING=mongodb://localhost:27017
```

## Setup
To run this project, install it locally using npm:
### Run Without Docker Compose

```
// clone the project
git clone https://github.com/RameshPrabakar/nodejs-mongo-ts-docker.git

// React Code
cd ui
npm install
npm start

// API code
cd api
npm install
npm run dev
```

## Docker compose

 * Let’s set up the development environment with Docker Compose. First, we need to install Docker Compose on your machine [here is the link](https://docs.docker.com/compose/install/).
 * MAke sure you have started docker and docker engine(runs by linux subsystem)
 * After installation you can use the following commands.
 
```
// build with no cache
docker-compose build --no-cache
// start the services
docker-compose up
// list the services
docker-compose ps
// list the containers
docker ps
// stop services
docker-compose stop
```

* After docker installation use `docker-compose up` cmd to start the application, ReactJs application will launch on your browser `https://localhost:8080`.





