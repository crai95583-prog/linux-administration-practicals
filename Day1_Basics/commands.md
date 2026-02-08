# Linux Practical - Day 1 Basics

## File & Directory Commands
- pwd → show current directory
- ls → list files
- mkdir test → create folder
- touch file.txt → create file

## Permissions
- chmod 755 file.sh
- chown user:user file.txt

## Process Management
- ps -ef
- top
- kill -9 PID

## Networking
- ping google.com
- netstat -tulnp
- ssh user@server-ip


## Disk Usage
- df -h → check total disk space
- du -sh * → check folder size

## Memory Usage
- free -m → check RAM usage

## CPU & System Info
- top → live process monitoring
- uname -a → kernel and OS details
- hostnamectl → system information



## View Logs
- tail -f /var/log/syslog → live log monitoring
- journalctl -xe → systemd logs and errors


## Search Text in Files
- grep "error" logfile.txt → find keyword in logs

## Find Files
- find / -name file.txt → search file in system



## Create Archive
- tar -cvf backup.tar folder/

## Extract Archive
- tar -xvf backup.tar

##  Key Learning
- Practiced Linux basics for DevOps administration and troubleshooting.



