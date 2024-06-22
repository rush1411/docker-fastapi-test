# docker-fastapi-test

Project Overview
This project demonstrates how to fork a GitHub repository, clone it, create a Dockerfile, and run the container.
The base image used for the Docker container is Python. The Dockerfile installs Python within the container.

Prerequisites:-
1.Git
2.Docker
3.A code editor VSCode

Forking and Cloning the Repository:-
1.Fork the Repository:

  1.Navigate to the original repository on GitHub.
  2.Click the "Fork" button on the top right to create a copy of the repository under your GitHub account.
  
2.Clone the Repository:

  1.Open terminal or Git Bash.
  2.Clone your forked repository using the following command:
bash
git clone https://github.com/rush1411/docker-fastapi-test

Creating the Dockerfile:-
1.Navigate to the root directory of your cloned repository.



Building and Running the Docker Container:-
  1.Build the Docker Image:

Run the following command in terminal from the root directory of your repository:

docker build -t your-image-name .

Run the Docker Container:-

After the image is built, run the container using the following command:-

docker run -p 4000:80 your-image-name
This maps port 80 in the container to port 4000 on your host machine.

Access Application:-

Open a web browser and go to http://localhost:8080 to see running application.

Docker Compose:-
If you prefer using Docker Compose, create a docker-compose.yml file in your repository root directory with the following content:

yaml
version: '3.0'

services:
  fastapi-test:
    container_name: nimap-fastapi-task
    image: rush1411/nimap-fastapi-task
    ports:
      - 8080:8080
    build: 
      dockerfile: ./Dockerfile
To use Docker Compose, run the following command:

docker-compose up

This will build and start your application in a Docker container using Docker Compose.
