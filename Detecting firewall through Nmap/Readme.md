This lab is created by ghanimah in order to capture the flag. 

NOTE: TAKE PERMISSION BEFORE USE NMAP TO YOUR CUSTOMER IN ORDER TO SCAN ANY WEB APPLICATION.

Detecting Firewalls 
The Nmap TCP ACK scan (-sA) will establish whether packets can pass through your firewall unfiltered. To speed up the scan, the –n option can be used to prevent reverse DNS resolution on the active IP addresses it finds

sudo nmap -sA 34.69.76.124 -p 21 --reason

IMPORTANT:If firewall is unblock it will show result as unfiltered and you will analazye in wireshark packets. 
otherwise,if firewall is block it will show filtered then no activity show in wireshark. 

Regards

Jamal H. Shah
