# Installing Docker on Different Platforms

Docker provides installation support for **Linux**, **Windows**, and **macOS**. Follow the steps below for your respective platform.

---

## **1. Installing Docker on Linux**
### Supported Distributions:
- Ubuntu
- Debian
- CentOS
- Fedora
- RHEL

### Steps:
1. **Update the package index**:
   ```
   bash
   
   sudo apt-get update
   sudo apt-get install ca-certificates curl gnupg lsb-release
   curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg


```
