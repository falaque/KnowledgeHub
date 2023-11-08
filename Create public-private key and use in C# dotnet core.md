* How to find format of the keys: https://vcsjones.dev/key-formats-dotnet-3/

Create public-private key:
==========================
follow: https://stackoverflow.com/questions/44474516/how-to-create-public-and-private-key-with-openssl

//generate private key:
``` openssl genrsa -out keypair.pem 2048 ```

//generate public key for above private key:
``` openssl rsa -in keypair.pem -pubout -out publickey.crt ```

Using these files in c#:
