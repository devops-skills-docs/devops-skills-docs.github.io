# Uncomplicated Firewall (ufw)
## Check status
```shell
sudo ufw status
```
### Verbose output
```shell
sudo ufw status verbose
```

## Enable ufw
Pay attention to not break ssh connectivity
```shell
sudo ufw enable
```

## Allow port
```shell
sudo ufw allow 22
```

## Allow port using specific protocol
```shell
sudo ufw allow 22/tcp
```
