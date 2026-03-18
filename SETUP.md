# Setup Guide

## Docker Setup

1. **Install Docker**: Download the Docker Desktop from [here](https://www.docker.com/products/docker-desktop) and install it.
2. **Clone the Repository**: 
   ```bash
   git clone https://github.com/princerenold2808-blip/IBRAHIM-.git
   cd IBRAHIM-
   ```
3. **Build the Docker Image**: Run the following command to build the Docker image:
   ```bash
   docker build -t ibrahim-app .
   ```
4. **Run the Docker Container**:
   ```bash
   docker run -p 3000:3000 ibrahim-app
   ```

## Manual Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/princerenold2808-blip/IBRAHIM-.git
   cd IBRAHIM-
   ```
2. **Install Dependencies**:
   ```bash
   npm install
   ```
3. **Start the Application**:
   ```bash
   npm start
   ```

## Configuration

- You may need to create a `.env` file in the root of the project with the following variables:
  ```dotenv
  DATABASE_URL=<your_database_url>
  PORT=3000
  ```

## Database Setup

1. **Install Database**: Make sure you have your database installed (e.g., PostgreSQL).
2. **Create a Database and User**:
   ```sql
   CREATE DATABASE ibrahim;
   CREATE USER ibrahim_user WITH ENCRYPTED PASSWORD 'yourpassword';
   GRANT ALL PRIVILEGES ON DATABASE ibrahim TO ibrahim_user;
   ```
3. **Run Migrations**: If applicable, run migrations to set up database schemas.

## Troubleshooting

- If you encounter issues, ensure:
  - Docker is running properly if using Docker.
  - All environment variables in `.env` are set correctly.
  - Database server is up and accessible.

## Features Overview

- **User Authentication**: Secure login and registration.
- **Responsive UI**: Works well on both desktop and mobile.
- **API Integration**: Connects seamlessly with external APIs for enhanced functionality.
- **Real-time Data**: Provides real-time updates using WebSocket.

---

For further assistance, please consult the documentation or open an issue in the repository.