# Dockerをインストールする手順

# Ubuntu
スーパーユーザーに移行  
```
sudo su
```
Dockerをインストール  
```
./ubuntu/install-docker.sh
```
再ログイン  

# Amazon linax 2023
gitをインストールする
```
sudo dnf update -y
sudo dnf install -y git
git --version
```

Dockerをインストールする
```
sudo dnf update -y
sudo dnf install -y docker
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
```
再ログイン
```
docker --version
```

Docker Composeをインストールする
```
sudo mkdir -p /usr/local/lib/docker/cli-plugins
curl -SL https://github.com/docker/compose/releases/download/v2.27.1/docker-compose-linux-x86_64 -o docker-compose
chmod +x docker-compose
sudo mv docker-compose /usr/local/lib/docker/cli-plugins/docker-compose
docker compose version
```
