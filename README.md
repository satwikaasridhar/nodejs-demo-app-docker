# nodejs-demo-app-docker
This project is a simple Node.js web application themed around shark conservation. It uses Bootstrap for responsive design and custom CSS for styling. The application features static pages like index.html and sharks.html, served using Express.js. It is fully Dockerized, allowing easy deployment via Docker Hub and execution on cloud platforms like AWS EC2. Ideal for beginners learning web development, Docker, and basic cloud deployment workflows.

# Node.js Sharks Demo

A simple Node.js web application showcasing a themed layout for a shark conservation website. The app is styled using Bootstrap and custom CSS, and is Dockerized for easy deployment.

## Features

- Express-based Node.js web server  
- Styled using Bootstrap and custom CSS  
- Jumbotron-style homepage with text and images  
- Dockerized for containerized deployment  
- Ready to be deployed to an EC2 instance or any Docker-compatible environment  

## Project Structure
node_project/ ├── app.js ├── package.json ├── views/ │   ├── index.html │   ├── sharks.html │   └── css/ │       └── styles.css └── Dockerfile

## Prerequisites

- Node.js  
- Docker  
- Git  

## Getting Started

### Run Locally

1. Clone Repository

2.Install dependencies:

npm install

3. Run the app:

node app.js

4. Visit http://localhost:8080 in your browser.

Run with Docker

1. Build Docker image:

docker build -t your_dockerhub_username/nodejs-image-demo .

2. Run the container:

docker run --name nodejs-image-demo -p 80:8080 -d your_dockerhub_username/nodejs-image-demo

3. Visit http://localhost to view the app.

**Deployment to EC2**

This app can be deployed to an AWS EC2 instance using Docker. Install Docker on your EC2 instance, pull your image from Docker Hub, and run the container using the same docker run command.
