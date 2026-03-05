## tcpdump
The tcpdump command is a packet sniffer and network security tool that captures real-time network packet information. 
Use the command to analyze traffic, troubleshoot issues, and monitor network security.
```shell
tcpdump [options] [filter]
```

### Example
- Server
```shell
tcpdump -i eth0 icmp
```
- Client
```shell
ping <server_eth0_ip>
```