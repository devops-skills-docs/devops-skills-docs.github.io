## Add Groups
```shell
sudo groupadd <groupname>
```

### Add user to group
```shell
sudo gpasswd --add <username> <groupname>
```
#### Short option
```shell
sudo gpasswd -a <username> <groupname>
```

### Remove user from group
```shell
sudo gpasswd --delete <username> <groupname>
```
#### Short option
```shell
sudo gpasswd -d <username> <groupname>
```

### Replace user login group 
```shell
sudo usermod --gid <new_login_group> <username>
```
#### Short option
```shell
sudo usermod -g <new_login_group> <username>
```

### Revert user login group 
```shell
sudo usermod --gid <username> <username>
```
#### Short option
```shell
sudo usermod -g <username> <username>
```
