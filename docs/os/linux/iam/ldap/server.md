## Lightweight Directory Access Protocol - LDAP
- [Intro](https://ubuntu.com/server/docs/introduction-to-openldap)

### Packages
- `slapd` - Stand-alone LDAP Daemon
### Abbreviations
- `dn` - Distinguished Name


- `.ldif` - LDAP Data Interchange Format
### Commands

#### generate passwords
```shell
slappasswd -c MD5 -s new_password
```

#### Validate Users
```shell
ldapwhoami -x -D cn=user1,ou=users,dc=<domain>,dc=com -W
```

#### See folder structure
```shell
ldapsearch -x -LLL -H ldap://localhost -b dc=<domain>,dc=com dn
```

#### See specific user
```shell
ldapsearch -x -LLL -b dc=<domain>,dc=com '(uid=john)'
```


#### Add Resource
```shell
   shell: ldapmodify -Y EXTERNAL -H ldapi:/// -f /tmp/add_ssl_options.ldif
```