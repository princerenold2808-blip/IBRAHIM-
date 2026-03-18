# Installation Guide for Online Pharmacy Application

This guide provides step-by-step instructions for setting up the Online Pharmacy Application locally using Docker.

## Prerequisites

Before you begin, ensure you have the following installed:
1. **Docker**: Download and install Docker from [Docker's official site](https://docs.docker.com/get-docker/).
2. **Docker Compose**: This is typically included with Docker Desktop installations. Check if it's installed by running `docker-compose --version`.

## Step 1: Clone the Repository

Open your terminal and run the following command to clone the repository:
```bash
git clone https://github.com/princerenold2808-blip/IBRAHIM- .
```

## Step 2: Navigate to the Project Directory

Change your directory to the cloned repository:
```bash
cd IBRAHIM-
```

## Step 3: Build the Docker Containers

Run the following command to build the Docker containers: 
```bash
docker-compose build
```

## Step 4: Start the Application

Use the following command to start the application:
```bash
docker-compose up
```

This command will start the application and its services, and you should see logs indicating that the services are up and running.

## Step 5: Access the Application

Once the application is running, open your web browser and navigate to:
```
http://localhost:3000
```

## Step 6: Stopping the Application

To stop the application, press `Ctrl + C` in the terminal where the application is running. You can also use:
```bash
docker-compose down
```

## Additional Commands

- To view running containers:
  ```bash
docker ps
  ```
- To remove all stopped containers:
  ```bash
docker container prune
  ```

## Conclusion

Follow these steps to set up the Online Pharmacy Application locally using Docker. For further queries or issues, refer to the project's GitHub Issues page or contact the maintainers.