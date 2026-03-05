## mount
All files accessible in a Unix system are arranged in one big tree, the file hierarchy, rooted at /. 

These files can be spread out over several devices. The mount command serves to attach the filesystem found on some 
device to the big file tree. Conversely, the umount(8) command will detach it again. 

The filesystem is used to control how data is stored on the device or provided in a virtual way by network or other services.

The standard form of the mount command is:
```shell
mount -t type device dir
```

This tells the kernel to attach the filesystem found on device (which is of type type) at the directory dir. 
The option -t type is optional. The mount command is usually able to detect a filesystem. 

The root permissions are necessary to mount a filesystem by default. See section "Non-superuser mounts" below for more details. 


The previous contents (if any) and owner and mode of dir become invisible, and as long as this filesystem remains mounted, 
the pathname dir refers to the root of the filesystem on device.

If only the directory or the device is given, for example:

```shell
mount /dir
```

then mount looks for a mountpoint (and if not found then for a device) in the /etc/fstab file. 
It's possible to use the --target or --source options to avoid ambiguous interpretation of the given argument. For example:

```shell
mount --target /mountpoint
```

The same filesystem may be mounted more than once, and in some cases (e.g., network filesystems) the same filesystem 
may be mounted on the same mountpoint multiple times. 

The mount command does not implement any policy to control this behavior. All behavior is controlled by the kernel and 
it is usually specific to the filesystem driver. 

The exception is --all, in this case already mounted filesystems are ignored (see --all below for more details).