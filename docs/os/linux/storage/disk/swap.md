```shell
swapon --show
```
## Provide swap partition
`<partition>` can have the format `sd[a-z][n]`, `vd[a-z][n]`, etc.
```shell
sudo mkswap /dev/<partition>
```
