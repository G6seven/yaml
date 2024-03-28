# Configuration Readme

## Docker Daemon Configuration

To modify the Docker daemon configuration, you can use the following command in your terminal:

```bash
nvim /etc/docker/daemon.json
{
  "data-root": "/RSP0/docker"
}
nvim /etc/hosts
network:
  version: 2
  renderer: networkd
  ethernets:
    enp5s0:
      addresses:
        - 192.168.9.100/24
        - 192.168.9.101/24
        - 192.168.9.103/24
        - 192.168.9.104/24
        - 192.168.9.105/24
        - 192.168.9.106/24
        - 192.168.9.107/24
        - 192.168.9.108/24
        - 192.168.9.109/24
        - 192.168.9.110/24
      gateway4: 192.168.9.1
      nameservers:
          addresses: [8.8.8.8, 1.1.1.1]


192.168.1.10 0
192.168.1.10 1  cloudflare ssh
192.168.1.10 2  portainer
192.168.1.10 3  pihole
192.168.1.10 4  lancache
192.168.1.10 5  octoprint
192.168.1.10 6  filecloud
192.168.1.10 7  kasm
192.168.1.10 8  minecraft server
192.168.1.10 9  CSGO
192.168.1.1 10
192.168.1.10
192.168.1.10
192.168.1.10

