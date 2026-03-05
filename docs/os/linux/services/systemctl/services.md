### List all services
```shell
systemctl list-units --type service --all
```

```shell
systemctl cat [servicename]
```
```shell
systemctl stop [servicename]
```

```shell
systemctl revert servicename
```
#### Disable a service
```shell
systemctl disable [--now] [servicename]
```

#### Reload all daemons
```shell
systemctl daemon-reload
```
#### Reset failed daemons
```shell
systemctl reset-failed
```

### Mask Services
```shell
systemctl mask [servicename]
```

```shell
systemctl unmask [servicename]
```
