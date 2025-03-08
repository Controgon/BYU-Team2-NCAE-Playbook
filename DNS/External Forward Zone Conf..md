/var/named/externalforward.db

```
$TTL 86400
@   IN  SOA ns1.team<T>.cyberjousting.org. admin.team<T>.cyberjousting.org. (
        2025022202  ; Serial
        3600        ; Refresh
        1800        ; Retry
        604800      ; Expire
        86400       ; Minimum TTL
)
@       IN  NS      ns1.team<T>.cyberjousting.org.
ns1     IN  A       172.18.10<T>.1
www     IN  A       172.18.10<T>.1
shell   IN  A       172.18.10<T>.2
files   IN  A       172.18.10<T>.2
```