# ctf-cheatsheet
Cheatsheet for common ctf problems

Albeit this is public repository it's mainly meant for private use so I do not need to google syntax for every snippet again and again. 


### Hydra
`hydra -t 16 -l <USERNAME> -P ../../rockyou.txt -vV <TARGET> ssh`

### Nmap
Basic CTF scan `nmap -oN=./nmap.txt -p- -sV -sC -vv <TARGET>`

## Steganography
[aperisolve.fr](https://aperisolve.fr/)

## Linux
Find SSUID executables `find / -perm -u=s -type f 2>/dev/null`

### Break out of app to get shell access 
https://gtfobins.github.io/

## Misc
Upgrade reverse shell to proper tty

```
python3 -c 'import pty; pty.spawn("/bin/bash")'
export TERM=xterm
Ctrl + Z
stty raw -echo; fg
```

