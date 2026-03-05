```shell
cat /etc/sudoers
```

## Add user to sudo group
```shell
sudo gpasswd -a <username> sudo
```

## Remove user from sudo group
```shell
sudo gpasswd -d <username> sudo
```

