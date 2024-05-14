# Configuration Readme

## Docker Containers Compose Files

To modify the Docker daemon configuration, you can use the following command in your terminal:

```bash
nvim /etc/docker/daemon.json
```

```bash
{
  "data-root": "/RSP0/docker"
}
```
## Nework Config 


```bash
network:
  version: 2
  renderer: networkd
  ethernets:
    enp5s0:
      addresses:
#        - 192.168.9.20/24
        - 192.168.9.100/24 # cloudflare ssh
        - 192.168.9.101/24 # portainer
        - 192.168.9.103/24 # pihole
        - 192.168.9.104/24 # lancache
        - 192.168.9.105/24 # octoprint
        - 192.168.9.106/24 # filecloud
        - 192.168.9.107/24 # kasm
        - 192.168.9.108/24 # mc-server
        - 192.168.9.109/24 # CSGO-server
        - 192.168.9.110/24

      gateway4: 192.168.9.1
      nameservers:
          addresses: [8.8.8.8, 1.1.1.1]
```

