### create key
```
openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -subj "/CN=xxxx/O=xxxxx/C=JP" -keyout ./sp.pem -out ./sp.crt

openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -subj "/CN=xxxx/O=xxxxx/C=JP" -keyout ./idp.pem -out ./idp.crt
```

### modify host file
```
127.0.0.1   sp.example.com
127.0.0.1   idp.example.com
```




