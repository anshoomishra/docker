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
