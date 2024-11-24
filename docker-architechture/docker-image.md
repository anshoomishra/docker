# Understanding Docker Architecture (cont...)

## Images, Containers, and Registries

Docker revolves around three fundamental components: **Images**, **Containers**, and **Registries**. These elements work together to enable containerized application development, deployment, and management.

---

### **1. Docker Images**

#### What are Docker Images?
- Docker images are **read-only templates** used to create containers.
- They contain everything needed to run an application, including:
  - Application code
  - Runtime environment
  - Dependencies
  - Libraries
  - Configuration files

#### Key Features:
- **Layered Structure**:
  - Built using multiple layers, where each layer represents a change (e.g., adding files or installing dependencies).
  - Layers are cached and reused to optimize storage and build performance.
  
- **Immutable**:
  - Once built, images cannot be modified.

#### Commands for Managing Images:
- **List images**:
```bash
  docker images
  docker pull <image-name>
  docker build -t <image-name> <build_context>
  docker rmi <image-name>

```

