🖥️ Simple System Monitoring Script
📌 Overview

This project provides a lightweight bash script that monitors system health (CPU, RAM, Disk, and Network).
It logs warnings when resource usage crosses defined thresholds.

🛠 Features

✅ Monitors CPU usage

✅ Monitors RAM usage

✅ Monitors Disk usage

✅ Checks Internet connectivity via ping

✅ Logs alerts with timestamps into a log file

⚡ (Optional) Can be extended to send email/SMS alerts

📂 Log File

All alerts are stored in:

/home/tushar/Projects/system_monitor.log


Example log entry:

[2025-09-17 18:45:23] High CPU Usage: 85%

⚙️ Configuration

You can change thresholds inside the script:

CPU_THRESHOLD=80   # CPU usage alert if above 80%
RAM_THRESHOLD=80   # RAM usage alert if above 80%
DISK_THRESHOLD=80  # Disk usage alert if above 80%

▶️ Usage

Make the script executable

chmod +x system_monitor.sh


Run the script manually

./system_monitor.sh


(Optional) Automate with cron
To run every 5 minutes:

crontab -e


Add this line:

*/5 * * * * /path/to/system_monitor.sh

🔧 Extend Features

Enable email alerts by uncommenting the mail line in CPU section.

Integrate with Slack/Telegram/Discord using webhooks.

Forward logs to centralized monitoring tools like ELK Stack / Grafana / Prometheus.

👨‍💻 Author

Tushar Srivastava
Project: System Monitoring (Linux Support)
