$TTL 86400
@   IN  SOA ns1.example.com. root.example.com. (
        2025022201  ; Serial
		3600      ; Refresh
        1800        ; Retry
        604800      ; Expire
        86400       ; Minimum TTL
)
@       IN  NS      ns1.example.com.
@       IN  NS      ns2.example.com.
ns1     IN  A       192.168.1.1
ns2     IN  A       192.168.1.2