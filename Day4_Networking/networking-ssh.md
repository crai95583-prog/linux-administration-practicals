# Linux Practical - Day 4 Networking & SSH

## ✅ Objective
To learn basic networking commands, remote access using SSH, and firewall checks in Linux.



## Check IP Address
```bash
ip a
or
ifconfig

## Test Network Connectivity
Ping a server:
ping google.com

## Check DNS resolution:
nslookup google.com

## Check Open Ports
List listening ports:
ss -tulnp

## Check Active Network Connections
netstat -an

## Download Data from Internet
curl ifconfig.me

wget https://example.com

## SSH Remote Login
Connect to remote server:
ssh user@server-ip


Example:

ssh ubuntu@13.233.xx.xx

## Secure Copy (SCP)
Copy file to remote server:
scp file.txt ubuntu@server-ip:/home/ubuntu/

Copy file from remote server:
scp ubuntu@server-ip:/home/ubuntu/file.txt .

## Firewall Status (UFW)
Check firewall status:
sudo ufw status

Allow SSH port:
sudo ufw allow 22

Allow HTTP port:
sudo ufw allow 80
