/etc/named.conf

```
zone "team<T>.cyberjousting.org" IN {
    type master;
    file "/var/named/externalforward.db";
};

zone "team<T>.net" IN {
    type master;
    file "/var/named/internalforward.db";
};

zone "10.168.192.in-addr.arpa" IN {
    type master;
    file "/var/named/internalreverse.db";
};

zone "10.18.172.in-addr.arpa" IN {
    type master;
    file "/var/named/externalreverse.db";
};
```