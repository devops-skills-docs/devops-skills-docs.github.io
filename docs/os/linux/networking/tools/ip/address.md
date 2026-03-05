## List IPs and network devices (Ethernet cards):
```shell
ip address/addr/a 
```

### Output Color
```shell
ip -c address/addr/a 
```

## Add Temporary ip to a NIC
```shell
sudo ip addr add <cidr> dev <nic>
```

## Remove Temporary IP from a NIC 
```shell
sudo ip addr delete <cidr> dev <nic>
```