# docker-samples

## ftp-sftp directory

Docker environments of ftp & sftp with docker-compose.yml.  
Passphrase is `mypassphrase` of `ftp-sftp/id_rsa_with_passphrase_key`.

### launch ftp, sftp server

```
docker-compose up
```

### sftp access

```
sftp -i id_rsa_with_passphrase_key -P 6022 testuser@127.0.0.1 # Use passphrase to 'mypassphrase'
sftp -i id_rsa_without_passphrase_key -P 6022 testuser@127.0.0.1
```

### ftp access

```
ftp bob@127.0.0.1 21 # Use password to 'bobpassword'
```

### shutdown ftp, sftp server

```
docker-compose down
```
