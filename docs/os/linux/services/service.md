## service
The service command in Linux is used to manage system services, which are long-running processes that are started 
at boot time and run in the background. 

These services are responsible for providing various system functionalities, such as networking, database management, and user authentication.

The service command is used to `start`, `stop`, `restart`, and `check the status` of these services. 

> It is a front-end to the systemctl command, which is used to manage the systemd service manager.

```shell
service <servicename> status
```

```shell
service <servicename> start
```

```shell
service <servicename> restart
```

```shell
service <servicename> stop
```