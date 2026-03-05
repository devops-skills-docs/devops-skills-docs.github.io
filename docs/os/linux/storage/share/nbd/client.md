## Network Block Devices (nbd) client 
```shell
sudo apt install nbd-client
```
#### Load for current lifecycle
```shell
sudo modprobe nbd
```
Load Permanently
```shell
echo nbd >> /etc/modules-load.d/modules.conf
```
### Connect
```shell
sudo nbd-client NBD_SERVER_FQDN_OR_IP -n <nbd_share_or_export_name>
```

```shell
sudo mount /dev/nbd0 /mnt
```

```shell
lsblk
```

## Disconnect
```shell
sudo umount /mnt
```

```shell
sudo ndb-client -d /dev/nbd0
```