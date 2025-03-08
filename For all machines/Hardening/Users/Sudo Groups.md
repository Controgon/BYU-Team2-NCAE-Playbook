sudo visudo

Look for content like below that allows the user 'munra' to execute any command

![[Pasted image 20250308005757.png]]

Any line that says something like this is also sus as it allows execution without a password prompt:
`<user/group> ALL=(ALL) NOPASSWD: ALL`