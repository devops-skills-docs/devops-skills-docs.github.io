## traceroute
- [Traceroute Man page](https://linux.die.net/man/8/traceroute)

The traceroute command is a networking diagnostics tool available for Linux, macOS, and Windows. 
The command tracks the route that packets take to reach a destination on a TCP/IP network.
Use the command to discover routing issues and bottlenecks by showing a packet's intermediate hops while traveling from source to destination.

The default trace is 30 hops with a packet size of 60 bytes for IPv4 (80 bytes for IPv6).
```shell
traceroute [options] [hostname/IP]
```