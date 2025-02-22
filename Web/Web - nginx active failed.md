sudo systemctl status nginx shows: 

![[Pasted image 20250222104212.png]]
and sudo systemctl start nginx shows:
![[Pasted image 20250222104541.png]]

Check sudo journal -xe

-says var/log/nginx doesnt exist
-so sudo mkdir /var/log/nginx
-then sudo systemctl restart nginx