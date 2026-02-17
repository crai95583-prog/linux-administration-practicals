# Linux Mini Project - Day 7 Server Health Monitoring

## ✅ Objective
To create a simple Linux server monitoring script that checks system health status.

This project simulates real DevOps daily monitoring tasks.

---

## 📌 Project Overview

The script will generate a health report including:

- CPU Load
- Memory Usage
- Disk Usage
- Uptime
- Running Services
- Recent Logs

---

## 1️⃣ Create Script File

```bash
nano health-check.sh


#!/bin/bash

echo "==============================="
echo "   Linux Server Health Report"
echo "==============================="

echo ""
echo "🕒 Uptime:"
uptime

echo ""
echo "📌 CPU Load:"
top -bn1 | head -5

echo ""
echo "💾 Memory Usage:"
free -m

echo ""
echo "🗄 Disk Usage:"
df -h

echo ""
echo "⚙️ Running Services (nginx example):"
systemctl status nginx --no-pager

echo ""
echo "📜 Recent System Logs:"
tail -n 10 /var/log/syslog

echo ""
echo "✅ Health Check Completed!"


3️⃣ Give Execute Permission
chmod +x health-check.sh

4️⃣ Run the Script
./health-check.sh
