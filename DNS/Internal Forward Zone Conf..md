```
$TTL 86400
@   IN  SOA ns1.team<T>.net. admin.team<T>.net. (
        2025022204  ; Serial
        3600        ; Refresh
        1800        ; Retry
        604800      ; Expire
        86400       ; Minimum TTL
)
@       IN  NS      ns1.team<T>.net.
ns1     IN  A       192.168.10<T>.2
www     IN  A       192.168.10<T>.3
db      IN  A       192.168.10<T>.4
```