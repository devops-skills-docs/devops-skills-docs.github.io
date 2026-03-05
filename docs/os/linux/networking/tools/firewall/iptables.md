## Allow SSH traffic
### Add Rule
```shell
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT
```

### Delete rule
```shell
sudo iptables -D INPUT -p tcp --dport 22 -j ACCEPT
```