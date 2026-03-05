- Server
```shell
 iperf3 -s -p <port>
```
- Client
```shell
iperf3 -c <server_ip> -p <port>
```

Specify connection numbers and time interval
```shell
iperf3 -t 10 -P 100 -c <server_ip> -p <port>
```