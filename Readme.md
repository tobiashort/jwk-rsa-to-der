```shell
Usage: jwk-rsa-to-der [JWK]
Reads from STDIN if JWK not provided as an argument.
		
Flags:
  -h	print help
exit status 1
```
To convert it into pem format:

```shell
cat example.json | jwk-rsa-to-der | openssl rsa -inform der -RSAPublicKey_in 
```