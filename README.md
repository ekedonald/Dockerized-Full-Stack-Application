# Full-Stack FastAPI and React Template

Welcome to the Full-Stack FastAPI and React template repository. This repository serves as a demo application for interns, showcasing how to set up and run a full-stack application with a FastAPI backend and a ReactJS frontend using ChakraUI.

## Project Structure

The repository is organized into two main directories:

- **frontend**: Contains the ReactJS application.
- **backend**: Contains the FastAPI application and PostgreSQL database integration.

Each directory has its own README file with detailed instructions specific to that part of the application.

## Getting Started

To get started with this template, please follow the instructions in the respective directories:

- [Frontend README](./frontend/README.md)
- [Backend README](./backend/README.md)


## Implementation of Dockerized Full Stack Web Application Deployment

After completing the steps above, the following steps are taken to dockerize the application:

### Step 1: Build a Frontend Image in the `frontend` Directory

- The Dockerfile should contain all the **Node** dependencies and executables needed to install and run the React application.

### Step 2: Build a Backend Image in the `backend` Directory

- The Dockerfile should contain all the  **Python Poetry** dependencies and executables needed run to Python application.

- Make the necessary changes in the `.env` files which will be referenced by `docker-compose` to build the application.

### Step 3: Create and Configure the `docker-compose.yml` file

- Move a step back in the directory and create the `docker-compose.yml` file.

- In the `docker-compose file`, reference the images and the Dockerfiles created in the backend and frontend directories.


### Step 4: Build and Run the Containerized Application

- Run the following command to build and the run the application:

```sh
docker-compose up -d
```

### Step 5: Verifying the Application

Go to your web browser and paste the following urls:

```sh
localhost
```

```sh
db.localhost
```

```sh
proxy.local host
```
