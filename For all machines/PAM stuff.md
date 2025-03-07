Look for password loggers

Look for recently modified files

Look in password auth and

Should be no perl, bash etc scripts in there (but look it up first)

PAM should only be compiled C stuff

Sudo lsof -I and netstat and ps aux | grep something

If find a running reverse shell look at the command and then search whole filesystem for that string

Sudo systemctl status cups