# Docker Containers

A **Docker container** is a lightweight, portable, and self-sufficient environment that runs an application. Containers are created from Docker images and provide isolation and consistency for running applications across different environments.

---

## **What is a Docker Container?**

- A **runtime instance** of a Docker image.
- Encapsulates an application and its dependencies in an isolated environment.
- Shares the host operating system kernel but runs independently from other containers.

---

## **Key Features of Docker Containers**

1. **Lightweight**:
   - Containers share the host operating system kernel, which reduces overhead compared to virtual machines.
   - Start and stop quickly, making them ideal for scaling applications.

2. **Portable**:
   - Run the same container image across different platforms (local, staging, production) without modification.

3. **Isolated**:
   - Each container has its own file system, processes, and network interfaces, ensuring no interference with other containers.

4. **Ephemeral or Persistent**:
   - Containers can be ephemeral (short-lived) or persistent with the help of volumes for data storage.

---

## **Lifecycle of a Docker Container**

1. **Create**:
   - A container is created from a Docker image.
```bash
   docker create <image-name>
   
```

2. **Start**:
   - The created container can be started to run the application.
```bash
   docker start <container-id>
   
```

3. **Run**:
   - Combines creation and starting of a container in one step.
```bash
   docker run <image-name>
   
```
4. **Stop**:
   - Running containers can be stopped.
```bash
   docker stop <container-id>
   
```

4. **Remove**:
   - Containers can be deleted when they are no longer needed.
```bash
   docker rm <container-id>
   
```