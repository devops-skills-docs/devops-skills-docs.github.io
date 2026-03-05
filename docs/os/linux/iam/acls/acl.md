## ACL - Access Control List
```shell
sudo apt install acl
```
## Set File Access Control List
```shell
sudo setfacl --modify user:<username>:<permissions> <filepath>
```
```shell
sudo setfacl --modify group:<groupname>:<permissions> <filepath>
```
### Remove permissions
```shell
sudo setfacl --modify user:<username>:--- <filepath>
```

## Get File Access Control List
```shell
sudo getfacl <filepath>
```

## Add Recursive
```shell
sudo setfacl --recursive --modify user:<username>:<permissions> <dirpath>
```

## Remove File Access Control List
```shell
sudo setfacl --remove user:<username> <filepath>
```
### Remove all
```shell
sudo setfacl --remove-all <filepath>
```

### Remove Recursive
```shell
sudo setfacl --recursive --remove user:<username> <dirpath>
```





