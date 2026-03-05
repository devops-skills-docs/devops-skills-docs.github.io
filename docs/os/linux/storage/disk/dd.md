# Disk Drives - [dd](https://man7.org/linux/man-pages/man1/dd.1.html)
- [Examples](https://blog.kubesimplify.com/the-complete-guide-to-the-dd-command-in-linux)

## Backup the entire hard disk
```shell
dd if=/dev/sda of=/dev/sdb
```

## Backup a Partition
```shell
dd if=/dev/hda1 of=~/partition.img
```

## create an image of a Hard Disk
```shell
dd if=/dev/hda of=~/hdadisk.img
```

## restore using the Hard Disk Image
```shell
dd if=hdadisk.img of=/dev/hdb
```
