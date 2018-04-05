Creating a Self-Signed SSL Certificate
```
openssl genres -des3 -out googleappsidp.key 2048
```

```
openssl rsa -in -out googleappsidp.key -out googleappsidp.pem
```
```
openssl req -new -key googleappsidp.key -out googleappsidp.csr
```

```
openssl x509 -req -day 9999 -in googleappsidp.csr -signkey googleappsidp.key -out googleappsidp.crt
```
