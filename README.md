
# How to connect to a ftp server using TLS
- Install ```lftp```
- Make a file with name ```.lftprc```
- Add below content in the file
```
set ftp:ssl-force true
set ftp:ssl-protect-list yes
set ftp:ssl-protect-data yes
set ftp:ssl-protect-fxp yes
set ssl:verify-certificate no
```
- Connect using command ```lftp username@hostname```
- Now you are connected to ftp server and can use all ftp commands
