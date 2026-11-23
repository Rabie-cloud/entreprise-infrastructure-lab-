Linux Service Management – Red Hat Enterprise Linux

1. Service Status

Checked SSH service status:

sudo systemctl status sshd

Result: active (running)

2. Service Startup Configuration

Checked whether SSH starts automatically:

sudo systemctl is-enabled sshd

Result: enabled

3. Service Restart

Restarted SSH service:

sudo systemctl restart sshd

Verified that the service was running successfully.

4. Running Services

Listed currently running services:

systemctl list-units --type=service --state=running

5. System Logs

Viewed the last 10 SSH service log entries:

sudo journalctl -u sshd -n 10

Skills Practiced

* Linux service administration
* systemctl commands
* SSH service monitoring
* Service startup configuration
* journalctl log analysis

Status: Successfully completed
