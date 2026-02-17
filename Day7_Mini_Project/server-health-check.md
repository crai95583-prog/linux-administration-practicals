# Linux Mini Project - Day 7 Server Health Monitoring

## ✅ Objective
To create a Linux server monitoring script that checks system health status.

This project simulates real DevOps daily monitoring tasks.

---

## 📌 Script Generates Report For

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
echo "⚙️ Running Services (SSH):"
systemctl status ssh --no-pager

echo ""
echo "📜 Recent System Logs:"
tail -n 10 /var/log/syslog

echo ""
echo "✅ Health Check Completed!"



chmod +x health-check.sh

./health-check.sh
