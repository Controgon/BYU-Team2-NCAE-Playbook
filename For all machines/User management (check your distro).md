
Change Passwords:
Blueteam, root

Check users:
sudo userdel -r username



Reset root or any passwords from grub:

Stop machine, repeadtly esc while starting

Press e

OG file:
![[Pasted image 20250307113029.png]]

Change to:

Ro to rw and at end init=/bin/bash. Possibly remove the maybe thing

Press ctl x or f10




Delete bad users

Don’t change passwords for scoring users – check these users for multiple ssh keys! Keep the one ending in SCORING

Check shadow, passwd for real sys users that have a shell but shouldn’t /sbin/nologin – run commands safer than edit file directly

SSH – look for extra dirs for keys other than .ssh/authorized_keys and keys2

Sudo passwd -l mail will lock account !! in :: in shadow (or diff in diff distro), then get rid of the bin bash above command: how to change a users shell