
check aliases = “alias”

exec bash top apply changes after changing ~/.bashrc or ~/.bash_aliases

To apply do source ~/.bashrc

Home user bashrc only changes for a single user

To find systemwide ones go to /etc/bashrc

Can also change to a different shell to avoid aliases while fixing them

If its not an alias then the binary files may be replaced – do which nano

There is a command to check integrity of the bins for everything (deb sum on ubuntu)