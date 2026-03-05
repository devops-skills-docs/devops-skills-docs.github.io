## Append
It will allow just append, no overwrite
```shell
sudo chattr +a <filepath>
```
### Disable append attribute
```shell
sudo chattr -a <filepath>
```

## Immutable
The file is frozen, can't be changed
```shell
sudo chattr +i <filepath>
```
