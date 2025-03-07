in /etc/shadow
Red team may change system users to be able to sign in and use shells. in shadows

Check for 
```
user::stuff
```

use

```
sudo usermod username
```
to disable the user from logging in, the corrected should look like the following:

```
user:!!:stuff

or

user:*:stuff
```

then check the user in /etc/passwd

```
user:stuff(/bin/bash)
```
or other versions of bash shells should be changed to 

```
user:stuff(/sbin/nologin)
```

through the command

```
sudo usermod --shell /bin/bash username
```