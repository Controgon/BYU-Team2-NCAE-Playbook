
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