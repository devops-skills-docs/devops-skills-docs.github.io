## Boot targets
```shell
systemctl get-default
```
### Permanent switch
Switch to GUI mode
```shell
systemctl set-default graphical.target
```

Switch to server mode
```shell
systemctl set-default multi-user.target
```

### Temporary switch
```shell
systemctl isolate graphical.target
```

### Other targets
- emergency.target
- rescue.target  