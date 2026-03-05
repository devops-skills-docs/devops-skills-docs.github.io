## Update users
```shell
sudo usermod --help
```

### Change user home directory
```shell
sudo usermod --home /home/<directory>/ --move-home <username>
```
#### Short option
```shell
sudo usermod -d /home/<directry> -m <username>
```

### Change user login
```shell
sudo usermod --login <old_username> <new_username>
```
#### Short option
```shell
sudo usermod -l <old_username> <new_username>
```

### Change user shell
```shell
sudo usermod --shell /bin/<shell> <username>
```
#### Short option
```shell
sudo usermod -s /bin/<shell> <username>
```

### Lock user
```shell
sudo usermod --lock <username>
```
#### Short option
Lock user login with password (mabe still able to login with ssh key)
```shell
sudo usermod -L <username>
```

### Unlock user
```shell
sudo usermod --unlock <username>
```
#### Short option
```shell
sudo usermod -U <username>
```

### Account Validity period
```shell
sudo usermod --expiredate <yyyy>-<mm>-<dd> <username>
```
#### Short version
```shell
sudo usermod -e <yyyy>-<mm>-<dd> <username>
```

### Remove account Validity period
Just pass an empty string
```shell
sudo usermod --expiredate "" <username>
```
#### Short version
```shell
sudo usermod -e "" <username>
```



