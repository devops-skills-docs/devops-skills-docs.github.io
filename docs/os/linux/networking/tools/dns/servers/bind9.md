# Berkley Internet Naming Daemon (BIND)

[DNS](https://ubuntu.com/server/docs/domain-name-service-dns)

Validation:
- ping:
  Ping needs to have reverse DNS setup properly. If you don’t have PTR records that point to your resources then `ping -a` won’t work. 
    ```shell
    ping -a IP/DNS
    ```