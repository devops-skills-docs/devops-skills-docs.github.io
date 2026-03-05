## Login as root
Can be used with root locked
```shell
sudo --login
```
### Short version
```shell
sudo -i
```
For users without root privileges, but we know the root password (`can't be used if root is locked`):
```shell
su -
```

```shell
su -l
```

```shell
su --login 
```

## Add root password
If root doesn't have a password, we can use:
```shell
sudo passwd root
```

## Lock root
```shell
sudo passwd --lock root
```
### Short version
```shell
sudo passwd -l root
```


## Unlock root
```shell
sudo passwd --unlock root
```
### Short version
```shell
sudo passwd -u root
```