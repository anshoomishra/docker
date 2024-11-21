
# Docker Tutorial Syllabus

## 1. Introduction to Docker
- [What is Docker?](./docker-introduction/what-is-docker.md)
- [Benefits of Docker](./docker-introduction/docker-benefits.md)
- [Docker vs. Virtual Machines](./docker-introduction/docker-vs-vm.md)
- [Installing Docker on Different Platforms (Linix, Mac, Windows)](./docker-introduction/docker-installation.md)

## 2. Understanding Docker Architecture
- Docker Engine
- Images, Containers, and Registries
- Docker CLI vs. Docker Desktop

## 3. Docker Basics
- Key commands:
  - `docker run`, `docker ps`, `docker stop`, `docker rm`
  - `docker pull`, `docker push`
- Working with Docker Hub
- Creating and running your first container

## 4. Docker Images
- What are Docker images?
- Understanding Dockerfile
- Building custom images (`docker build`)
- Best practices for Dockerfiles
- Managing images (`docker images`, `docker rmi`)

## 5. Docker Containers
- Lifecycle of a container
- Accessing containers via `docker exec`
- Persisting data with volumes
- Networking in Docker containers
- Linking containers

## 6. Docker Compose
- What is Docker Compose?
- Writing `docker-compose.yml` files
- Multi-container applications
- Running and managing with `docker-compose up/down`

## 7. Docker Networking
- Default Docker networks
- Creating custom networks
- Bridged, host, and overlay networks
- Container-to-container communication

## 8. Docker Volumes
- Bind mounts vs. volumes
- Sharing data between containers
- Backing up and restoring volumes

## 9. Docker Registry
- Setting up a private Docker registry
- Managing images in a registry
- Security best practices for registries

## 10. Docker for Development
- Using Docker in development workflows
- Debugging in Docker containers
- Docker with CI/CD pipelines
- Using Docker with GitHub Actions

## 11. Docker for Production
- Optimizing images for production
- Security best practices
- Monitoring containers
- Auto-scaling containers

## 12. Advanced Docker Topics
- Multi-stage builds
- Docker Secrets for sensitive data
- Using Docker in microservices architecture
- Troubleshooting Docker containers

## 13. Kubernetes and Docker
- Introduction to Kubernetes
- Docker's role in Kubernetes
- Transitioning from Docker Compose to Kubernetes manifests

## 14. Hands-On Projects
- Building a Node.js application with Docker
- Creating a LAMP stack with Docker Compose
- Deploying a full-stack application
- Setting up a WordPress blog with Docker and Nginx
