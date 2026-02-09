# Linux Practical - Day 2 Package & Service Management

## ✅ Objective
To understand how to install, update, remove packages and manage services in Linux.

---

## 1️⃣ Update System Packages

```bash
sudo apt update
sudo apt upgrade -y

## Install a Package (Example: Nginx)
sudo apt install nginx -y

## Check installed version
nginx -v


## Check service status:
systemctl status nginx

## Start service:
sudo systemctl start nginx

## Enable service at boot:
sudo systemctl enable nginx

## Restart service:
sudo systemctl restart nginx

## Stop service:
sudo systemctl stop nginx

## Check process:

ps -ef | grep nginx


## Check open ports

ss -tulnp | grep nginx

## Remove Package
sudo apt remove nginx -y
sudo apt autoremove -y

