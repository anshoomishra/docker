# Docker Registries

A **Docker Registry** is a centralized repository for storing and distributing Docker images. It acts as the bridge between developers and runtime environments, enabling easy sharing, versioning, and deployment of container images.

---

## **What is a Docker Registry?**

- A **registry** stores Docker images, which can be pulled by Docker clients to create containers.
- Acts as a hub for developers to share prebuilt images or host their custom images for deployment.

---

## **Types of Docker Registries**

1. **Public Registries**:
   - Open to everyone and often free.
   - Examples:
     - [Docker Hub](https://hub.docker.com) (default registry for Docker)
     - [GitHub Container Registry](https://github.com/features/packages)
   - Hosts millions of prebuilt images for various applications and frameworks.

2. **Private Registries**:
   - Restricted access, used within organizations for proprietary applications.
   - Examples:
     - AWS Elastic Container Registry (ECR)
     - Google Container Registry (GCR)
     - Harbor (open-source registry)

---

## **Key Features of Docker Registries**

1. **Image Versioning**:
   - Registries support image tags to manage different versions.
   - Example:
     ```bash
     docker pull nginx:1.21.6
     ```

2. **Access Control**:
   - Private registries allow organizations to control who can push or pull images.

3. **Caching**:
   - Speeds up builds and deployments by caching frequently used images locally.

---

## **Basic Commands for Docker Registries**

1. **Login to a Registry**:
```bash
   docker login

```

2. **Pull an Image**:
- Developers or systems pull images from a registry to use them locally.
```bash
   docker pull nginx:latest
   docker pull ubuntu:latest

```

3. **Push an Image**:
- Developers push their built images to a registry for sharing or deployment.
```bash
  docker tag myapp:1.0 username/myapp:1.0
  docker push username/myapp:1.0 
  docker push username/myapp:latest

```

4. **Search for an Image:**

```bash
docker search <image-name>
```

## Diagram: Docker Registries, Images, and Containers

```plaintext
+------------------+       +------------------+
|   Docker Image   | <---> | Docker Registry  |
+------------------+       +------------------+
         ^
         |
         v
+------------------+
| Docker Container |
+------------------+
