# How to connect to a ftp server using TLS

1. Install ```lftp```
2. Make a file with name ```.lftprc```

```set ftp:ssl-auth TLS
set ftp:ssl-force true
set ftp:ssl-protect-list yes
set ftp:ssl-protect-data yes
set ftp:ssl-protect-fxp yes
set ssl:verify-certificate no```

3. Connect using command
```lftp username@hostname```
