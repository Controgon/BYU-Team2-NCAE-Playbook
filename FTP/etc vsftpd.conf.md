change local_root to =/mnt/files

make sure ownership of directories and files are appropritate (eg make a group with the neccessary users in it and then set ownership to ftp:ftpusers)


vsftpd.conf
```
anonymous_enable=NO
local_enable=YES
write_enable=YES
local_umask=022
chroot_local_user=YES
allow_writeable_chroot=YES
```
