# Private Docker Registry

Set up a private docker repository.

## Getting Started

### Configuration

Add/update the daemon.json in /etc/docker/daemon with the following

```
{
    "insecure-registries":[
        "localhost:5000"
    ]
}
```

Reload Docker daemon

```
sudo systemctl daemon-reload
```

Restart docker

```
sudo systemctl restart docker
```

Run docker compose

```
docker-compose up -d
```
