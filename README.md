# Crypto Monitoring Application

A real-time cryptocurrency price monitoring application with price alerts.

## Tech Stack

- Frontend: React
- Backend: Node.js with Express
- Database: MongoDB
- Cache: Redis

## Docker Setup

The application is fully dockerized with the following services:
- Frontend (React)
- Backend (Node.js)
- MongoDB
- Redis

### Prerequisites

- Docker
- Docker Compose

### Running the Application

1. Clone the repository
2. Navigate to the project directory
3. Run the following command:
   ```bash
   docker-compose up --build
   ```

### Accessing Services

- Frontend: http://localhost:3000
- Backend API: http://localhost:4000
- MongoDB: localhost:27017
- Redis: localhost:6379

### Development

The application uses Docker volumes for development:
- MongoDB data is persisted in a named volume
- Source code changes are reflected immediately due to volume mounts

### Stopping the Application

To stop the application:
```bash
docker-compose down
```

To stop and remove volumes:
```bash
docker-compose down -v
```
