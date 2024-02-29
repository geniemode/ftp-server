
# How to connect to a ftp server using TLS
1. Install ```lftp```
1. Make a file with name ```.lftprc```
1. Add below content in the file
```
set ftp:ssl-force true
set ftp:ssl-protect-list yes
set ftp:ssl-protect-data yes
set ftp:ssl-protect-fxp yes
set ssl:verify-certificate no
```
1. Connect using command ```lftp username@hostname```
