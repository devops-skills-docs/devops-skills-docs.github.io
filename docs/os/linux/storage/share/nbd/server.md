## Network Block Devices (nbd) server

```shell
sudo apt install nbd-server
```

```shell
sudo nano /etc/nbd-server/config
```

```ini
[generic]
user = nbd
group = nbd
includedir = /etc/nbd-server/conf.d
allowlist = true

[partition2]
exportname=/dev/sda1
```

```shell
sudo systemctl restart nbd-server.service
```