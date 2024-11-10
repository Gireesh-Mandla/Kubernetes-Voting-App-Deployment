# Kubernetes Voting App Deployment

This project demonstrates the deployment of a scalable voting application using Kubernetes. The app consists of multiple microservices, including a frontend for user voting, a Redis server for real-time vote caching, and a backend database to store voting results.

## Architecture Overview

The application follows a multi-tier microservices architecture:

- **Frontend Service**: User interface for voting.
- **Redis Server**: Caching layer for real-time votes.
- **Backend API**: Processes votes and interacts with the database.
- **Database**: Stores voting results for long-term data persistence.

## Features

- **Scalable Microservices**: Each component (frontend, Redis, backend, database) is containerized with Docker.
- **Kubernetes Orchestration**: Services are managed by Kubernetes, ensuring high availability and easy scaling.
- **Real-Time Caching with Redis**: Redis provides low-latency storage for incoming votes.
- **Persistent Storage**: Persistent Volumes (PV) and Persistent Volume Claims (PVC) ensure data persistence for the database.

## Project Workflow

1. **Containerization**: Each service is built as a Docker container, stored in a container registry.
2. **Kubernetes Configuration**: Defined with YAML files for deployments, services, and persistent storage.
3. **Scalability**: The app is tested to scale efficiently by dynamically adjusting pod counts.
4. **Monitoring**: Prometheus and Grafana track application health, resource usage, and performance.

## Setup and Deployment

### Prerequisites

- Kubernetes Cluster
- kubectl CLI
- Docker
- Helm (optional, for managing Kubernetes applications)

### Deployment Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/username/Kubernetes-Voting-App-Deployment.git
   cd Kubernetes-Voting-App-Deployment
