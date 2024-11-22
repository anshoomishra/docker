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
1. **Update the package index:**
```bash
sudo apt-get update
```
2. **Install required packages:**
```bash
sudo apt-get install ca-certificates curl gnupg lsb-release
```   
3. **Add Docker's official GPG key:**   
```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

```
4. **Set up the stable repository:**   
```bash
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

```

5. **Install Docker Engine:**   
```bash
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io

```


6. **Verify Docker installation:**   
```bash
docker --version

```

## **2. Installing Docker on Windows**

### Steps:

1. **Download Docker Desktop:**

- Visit the Docker Desktop for Windows page and download the installer.

2. **Run the Installer:**

- Double-click the downloaded .exe file.
- Follow the installation wizard to install Docker Desktop.

3. **Enable WSL 2:**   

- Docker Desktop requires the Windows Subsystem for Linux (WSL 2).
- Run the following commands in PowerShell:

```bash
wsl --install

```
4. **Restart your system:**   

5. **Verify installation**
- Open a terminal and run:
```bash
docker --version

```
## **3. Installing Docker on macOS**

### Steps:

1. **Download Docker Desktop:**   

- Visit the Docker Desktop for macOS page and download the installer.

2. **Run the Installer:**  

- Double-click the downloaded .dmg file.
- Drag the Docker icon to the Applications folder.

3. **Start Docker Desktop:**   

- Open Docker Desktop from the Applications folder.
- Follow the setup instructions.

4. **Verify installation:** 

- Open a terminal and run:

```bash 

docker --version

```

## **Post-Installation Steps**

### **For Linux:**

- Manage Docker as a non-root user:

```bash

sudo groupadd docker
sudo usermod -aG docker $USER

```