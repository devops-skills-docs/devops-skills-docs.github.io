## netstat
The netstat command (network statistics) is a networking utility that shows various networking statistics. 
The command provides statistics for network ports and shows port availability.

The command is part of the `net-tools` package and is considered `obsolete`. The recommended replacement is the `ss` 
command, which is part of `iproute2`. Other functionalities of the netstat command are available with the `ip` command.

### Install
```shell
sudo apt install net-tools
```

### Syntax
```shell
netstat [options]
```

### Example
```shell
netstat -n
```
