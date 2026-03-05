## NFS server
### Install
```shell
sudo apt install nfs-kernel-server
```

### Configure
```shell
man exports
```

```shell
sudo nano /etc/exports
```

| Path          | Host(Permissions)                                                       |
|---------------|-------------------------------------------------------------------------|
| /srv/[subdir] | host1.example.com(rw,sync,no_subtree_check) IP(ro,async,no_root_squash) |


## Apply changes
```shell
man exportfs
```
```shell
sudo exportfs -r
```
