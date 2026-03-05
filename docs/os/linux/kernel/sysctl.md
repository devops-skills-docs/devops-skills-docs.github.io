# Kernel runtime parameters
```shell
sysctl -a
```

```shell
sudo sysctl -a
```
## See one parameter
```shell
sudo sysctl <parameter>
```

Write parameter for this session:
```shell
sudo sysctl -w <parameter>=<value>
```

See all *.conf
```shell
ls -a /etc/sysctl.d/
```

## Add persistent changes
Create new *.conf file
```shell
sudo nano /etc/sysctl.d/swap-less.conf 
```
and add the desired change
```text
vm.swapiness=20
```
In order to `apply those changes right away`, and not wait for the next reboot,
```shell
sudo sysctl -p /etc/sysctl.d/swap-less.conf
```

```shell
suso nano /etc/sysctl.conf
```
