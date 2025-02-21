## Get Certificates
```
/certificate print
```
Prints the certificates, should start as empty

## Add Certifcate
```
/certificate add name=Server_name common-name=server_name
```
## Sign the New Certificate
Required
```
/certificate sign Server_name
```

## Get More Detail on Cert
```
/certificate print detail
```

## Enable HTTPS
```
/ip service enable www-ssl
```

## Set it to Use the Certificate
```
/ip service set www-ssl certificate=Server disabled=no
/ip service set www-ssl 
```

