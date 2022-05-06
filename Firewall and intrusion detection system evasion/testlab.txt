This lab is created by ghanimah.com in order to capture the flag (ethical hacking course)

NOTE: TAKE PERMISSION BEFORE USE NMAP TO YOUR CUSTOMER IN ORDER TO SCAN ANY WEB APPLICATION.

sudo nmap -sS  -sV -D 120.9.0.0,98.8.6.9,23.65.67.21 icebreakerspro.com

Send different packets with different ip in order manupulation to the target . Target will individual check all ip if ip is down then this is will fake ip it will block in order to safe from attack. 

if will add this  in  last (ME) then it will show real ip in wireshark in the end (Less use by nmap the real ip in order to avoid to show in wirehark)

sudo nmap -sS  -sV -D 120.9.0.0,98.8.6.9,23.65.67.21,me icebreakerspro.com 

Regards
Jamal H. Shah
