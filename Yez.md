Pre-install process
### Wsl
```bash
wsl --install -d Ubuntu-24.04
```
```bash
wsl --list --verbose
```
### Docker
```bash
sudo apt-get update
```
```bash
sudo apt-get install -y ca-certificates curl gnupg
```
```bash
sudo install -m 0755 -d /etc/apt/keyrings
```
```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/ keyrings/docker.gpg
```
```bash
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```
```bash
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
```bash
sudo apt-get update
```
```bash
sudo apt-get install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
```bash
sudo usermod -aG docker $USER
```
```bash
docker run hello-world
```
### Git
```bash
sudo apt-get update
```
```bash
sudo apt-get install -y git
```
```bash
git --version
```
### Hard drive 
```bash
cd ~krpc
```
```bash
tar -xvf krpc7th-simulator.tar.gz
```
```bash
docker load --input intball-simulator.tar
```
Hope it runs



