## Storage monitoring
```shell
apt install sysstat
```

### iostat

```shell
iostat
```

#### Show just device utilization (no cpu)
```shell
iostat -d
```

#### Human-readable output
```shell
iostat -h
```
#### See all partitions
```shell
iostat -p ALL
```
#### See just a partition
```shell
iostat -p sda
```


#### Refresh io statistics every 5 seconds
```shell
iostat 5
```

### pidstat

```shell
pidstat -d
```
#### Refresh pid statistics every 5 seconds

```shell
pidstat -d 5 
```

### dmsetup
```shell
sudo dmsetup info /dev/dm-0
```
