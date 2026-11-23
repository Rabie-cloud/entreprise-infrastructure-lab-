Linux Firewall and SELinux Lab

Environment

* OS: Red Hat Enterprise Linux
* Network Interface: ens160
* Firewall: firewalld
* SELinux: Enabled

1. Firewall Management

Check Firewall Status

sudo firewall-cmd --state

Result: running

Check Active Zone

sudo firewall-cmd --get-active-zones

* Active zone: public
* Interface: ens160

Check Allowed Services

sudo firewall-cmd --list-all

Allow HTTP and HTTPS

sudo firewall-cmd --add-service=http --permanent
sudo firewall-cmd --add-service=https --permanent
sudo firewall-cmd --reload

Verify Configuration

sudo firewall-cmd --list-services

Result: HTTP and HTTPS services were successfully added and verified.

2. SELinux Management

Check SELinux Mode

getenforce

Result: Enforcing

Check SELinux Status

sudo sestatus

Verified:

* SELinux status: Enabled
* Current mode: Enforcing
* Policy type: Targeted

3. Skills Practiced

* Linux firewall management
* firewalld service configuration
* HTTP and HTTPS firewall rules
* Active firewall zones and interfaces
* SELinux status verification
* Linux security fundamentals

Conclusion

Successfully configured and verified firewall rules and checked SELinux security status on Red Hat Enterprise Linux.

Note: Firewall rules were configured and verified. No web server deployment or HTTP connectivity test was performed.
