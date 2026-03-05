# ss
- [ss Man Page](https://man7.org/linux/man-pages/man8/ss.8.html)

The ss command is a CLI tool for displaying network statistics. The tool is part of the iproute2 package and is a faster alternative to the netstat command.

Use the ss command to examine network sockets and view various network-related data.
```shell
ss [options] [filter]
```
It will replace netstat.
```shell
ss --help
```

```shell
sudo ss -ltunp
```

```shell
netstat -ltunp
```