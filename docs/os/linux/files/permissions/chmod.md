## chmod
Change file mode bits

[](https://en.wikipedia.org/wiki/Chmod#Special_mode)

### Add user execute permission
```shell
chmod u+x <filepath>
```
### Add user write and world readable permissions
```shell
chmod 644 <filepath>
```
same as
```shell
chmod a=r,u+w foo
```

### Add user rw permissions recursive
```shell
chmod -R u+rw <dirpath>
```