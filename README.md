# docker-samples

## ftp-sftp directory

Docker environments of ftp & sftp with docker-compose.yml.  
Passphrase is `mypassphrase` of `ftp-sftp/id_rsa_with_passphrase_key`.

You can access After docker-compose up.

```
sftp -i id_rsa_with_passphrase_key -P 6022 testuser@127.0.0.1
sftp -i id_rsa_without_passphrase_key -P 6022 testuser@127.0.0.1  # (Use 'mypassphrase')
```
