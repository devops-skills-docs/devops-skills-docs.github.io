## Manage password 
```shell
sudo passwd <username>
```

### Set password validity period
```shell
sudo chage --lastday 0 <username>
```
#### Short option
```shell
sudo chage -d 0 <username>
```

### Un-expire password
```shell
sudo chage --lastday -1 <username>
```
#### Short option
```shell
sudo chage -d -1 <username>
```

### Expire password in 30 days
```shell
sudo chage --maxdays 30 <username>
```
#### Short option
```shell
sudo chage -M 30 <username>
```

### Set password to never expire
```shell
sudo chage --maxdays -1 <username>
```
#### Short option
```shell
sudo chage -M -1 <username>
```

### Check when the password expire
```shell
sudo chage --list <username>
```
#### Short option
```shell
sudo chage -l <username>
```