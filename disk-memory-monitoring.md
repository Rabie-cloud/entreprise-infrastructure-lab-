Linux Disk and Memory Monitoring – Red Hat Enterprise Linux

1. Disk Space Monitoring

Checked filesystem disk usage:

df -h

Displayed disk space in human-readable format.

2. Memory Monitoring

Checked RAM usage:

free -h

Reviewed total, used, free and available memory.

3. Block Devices

Listed disks and partitions:

lsblk

Checked filesystem and mountpoint information:

lsblk -f

4. Log Directory Size

Checked total log directory size:

sudo du -sh /var/log

Result: Approximately 11 MB.

Skills Practiced

* Disk space monitoring
* RAM monitoring
* Linux block devices
* Filesystem inspection
* Log storage analysis

Status: Successfully completed
