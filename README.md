# Dockerをインストールする手順

# Ubuntu
ubuntu/install-docker.shを実行

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
sudo dnf update
sudo dnf install docker-compose-plugin
docker compose version
```
