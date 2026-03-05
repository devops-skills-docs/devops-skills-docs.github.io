## Last Log 

The lastlog command in Linux displays the most recent login time, terminal, 
and source host for all users or a specific user by reading the /var/log/lastlog file. 

It is useful for security auditing and identifying inactive accounts. 
The command sorts output by User ID (UID) and indicates users who have "Never logged in"

```sh
cat /var/log/lastlog
```

### Show all users' last login: 
```sh
lastlog
```

### Show a specific user's last login: 
```sh
lastlog -u <username>
```

### Show logins within a specific number of days: 
```sh
lastlog -t <days> (e.g., lastlog -t 7 for the last week)
```

### Show logins before a specific number of days: 
```sh
lastlog -b <days>
```

### Clear a user's lastlog record: 
```sh
lastlog -u <username> -C (requires root) 
```