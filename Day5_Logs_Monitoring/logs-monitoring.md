# Linux Practical - Day 5 Logs, Monitoring & Troubleshooting

## ✅ Objective
To learn how to monitor system resources, analyze logs, and troubleshoot issues in Linux servers.

---

#### System Monitoring Commands

### Check CPU & Processes

```bash
top
htop
ps -ef

Check Memory Usage
free -m

Check Disk Usage
df -h
du -sh *

##### Log Monitoring (Very Important)
 View system logs
tail -f /var/log/syslog

Check authentication logs
cat /var/log/auth.log

View error logs using journalctl
journalctl -xe

## Search Logs for Errors
grep "error" /var/log/syslog
grep "failed" /var/log/auth.log

## Check Running Services
List all services
systemctl list-units --type=service

Check specific service status
systemctl status nginx

  ## Network Troubleshooting
Check open ports
ss -tulnp

Test connectivity
ping google.com
curl -I google.com

## Troubleshooting Use Case Examples
Server Disk Full
df -h
du -sh /var/log/*

Service Not Running
systemctl restart nginx
systemctl status nginx

High CPU Usage
top
ps -eo pid,ppid,cmd,%mem,%cpu --sort=-%cpu | head
