Repository Name: Server Resource Utilization Monitor

Description:
This repository contains a Python-based monitoring tool designed to track critical system resources like CPU, memory, disk, and swap usage on Linux servers. The script logs spikes in utilization and sends email alerts when resource usage exceeds 95%, along with details about the top processes causing high usage. It also sends follow-up alerts when resource utilization returns to normal. This tool helps administrators monitor server health and detect resource bottlenecks proactively.

Key Features:
Real-time Monitoring: Continuously monitors CPU, memory, disk, and swap usage.
Threshold Alerts: Sends email notifications if any resource usage exceeds 95%.
Top Process Details: Captures and logs the top 5 processes by CPU and memory utilization during spikes.
Auto-logging: Logs spike details with timestamps and resource usage in a file for historical analysis.
Normalization Alerts: Sends follow-up emails once the resource usage returns to normal.
Customizable: Adjustable monitoring intervals and thresholds based on server requirements.
HTML Email Alerts: Provides detailed, formatted HTML email notifications for easier readability.

Technologies:
Python: Primary language used for scripting.
psutil: Python library for system and process utilities.
smtplib: Standard library for sending email notifications via SMTP.
Linux-based systems: Designed for Red Hat Enterprise Linux (RHEL) and similar Unix/Linux environments.

Clone the repository:

git clone https://github.com/your-repo-name/server-resource-monitor.git
cd server-resource-monitor

Install the required libraries:

pip install psutil

Modify the script to fit your environment:

Update sender and recipient email addresses.
Ensure the SMTP mail relay server is configured correctly.
Run the script:

python3 resource_monitor.py
(Optional) Schedule the script as a cron job for continuous monitoring.

Contributions:
Feel free to fork the repository and submit pull requests. Contributions and improvements are always welcome!

License:
This project is licensed under the MIT License – see the LICENSE file for details.
