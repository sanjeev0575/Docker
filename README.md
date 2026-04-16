# docker compose install on amazon liunx 

```
sudo dnf install -y docker
```

## Start Docker

```
sudo systemctl start docker
sudo systemctl enable docker

```

## Docker compose installation

```
mkdir -p ~/.docker/cli-plugins

curl -SL https://github.com/docker/compose/releases/latest/download/docker-compose-linux-x86_64 \
-o ~/.docker/cli-plugins/docker-compose

chmod +x ~/.docker/cli-plugins/docker-compose

```

# docker-compose version

```
docker-compose version
```

# Quick workaround (if you want immediate run)

```
export DOCKER_BUILDKIT=0
docker-compose up -d

```