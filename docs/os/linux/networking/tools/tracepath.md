## tracepath
- [Tracepath Man Page](https://linux.die.net/man/8/tracepath)

The tracepath command is similar to the traceroute command. The command identifies paths and latencies from source to 
destination, mapping the router and network hops.

Although traceroute is a well-known command with comprehensive options, the tracepath command is a simple network 
mapping tool available on most Linux systems.
```shell
tracepath [options] [hostname/IP]
```

```shell
man tracepath
```

It traces path to destination
```shell
tracepath <destination> -m 10 -p 443
```