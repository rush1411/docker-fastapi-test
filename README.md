# docker-fastapi-test

Steps to Run the Project
1. Clone the Repository
Clone the repository from GitHub to your local machine:

git clone https://github.com/rush1411/docker-fastapi-test.git

2. Navigate to the Project Directory
Change to the project directory:

cd docker-fastapi-test

4. Build or Pull the Docker Image
You have two options to get the Docker image:

a) Build the Image Locally
Use the following command to build the Docker image locally:


docker compose build
b) Pull the Image from Docker Hub
Alternatively, you can pull the pre-built image from Docker Hub:

docker pull rush1411/nimap-fastapi-task

4. Run the Container Using Docker Compose
Start the container using the docker-compose.yml file:

docker compose up -d

The -d flag runs the container in detached mode.

5. Stop the Running Container
To stop and remove the running containers, use the following command:

docker compose down

Following these steps will help you set up and run the project efficiently.
