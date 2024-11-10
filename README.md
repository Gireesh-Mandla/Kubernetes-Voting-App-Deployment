Kubernetes Voting App Deployment

In this project, I designed and deployed a scalable, containerized voting application using Kubernetes. The app consists of a frontend for users to vote, a Redis server for managing votes in real-time, and a backend database to store the voting results. The deployment was orchestrated on Kubernetes clusters to ensure high availability and resilience under load.

Key Features:
Multi-Tier Architecture: Separated frontend, backend, and database services, enabling scalable microservice deployment.
Redis Caching: Used Redis for handling real-time voting data with low latency.
Dockerized Microservices: Each component (frontend, backend, Redis, and database) was containerized using Docker for consistent deployment across environments.
Kubernetes Orchestration: Utilized Kubernetes for managing, scaling, and load balancing the application, with services, deployments, and pods to ensure optimal resource utilization.
Configurable Storage: Integrated persistent volume storage for database reliability and data retention during pod failures.
Deployment Workflow:
Containerization: Developed Docker images for each service and uploaded them to a container registry.
Kubernetes Setup: Defined deployment YAML files for services, deployments, and pods to ensure a reproducible and stable setup.
Scalability Testing: Tested scaling capabilities to handle traffic surges by dynamically adjusting the number of pods.
Monitoring & Logging: Implemented monitoring using Prometheus and Grafana to track resource usage, response time, and error rates.
Outcome:
The Kubernetes Voting App provides a robust example of how containerization and orchestration can simplify complex application deployments while enhancing scalability and reliability. This project also improved my skills in microservices architecture, Docker, and Kubernetes management.
