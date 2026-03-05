```shell
sudo apt install libnns-ldapd
```
> the package is `libnns-ldapd`, NOT `libnns-ldap`

- NSS = Name Server Switch
- nslcd = Name Service Local Daemon

Steps : 
1. Configure ldap server URI, `ldap://<ldap_server_ip>/`
2. Configure search base `dc=domain,dc=com`
3. Name services to configure:
  - [x] passwd
  - [x] group
  - [x] shadow
  - [ ] hosts
  - [ ] networks
  - [ ] ethers
  - [ ] protocols
  - [ ] services
  - [ ] rpc
  - [ ] netgroup
  - [ ] aliases


```shell
cat /etc/nsswitch.conf
```

```shell
sudo cat /etc/nslcd.conf
```
### Get entries from all sources
```shell
getent passwd
```
### Get entries from ldap server
```shell
getent passwd --service ldap
```

### Get groupd from ldap server
```shell
getent groups --service ldap
```