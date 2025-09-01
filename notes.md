# My Notes



\# Linux \& Networking Cheat-Sheet



\## 🔹 Basic Linux Commands

\- `pwd` → Print working directory  

\- `ls -l` → List files with details (permissions, owner, size)  

\- `cd <dir>` → Change directory  

\- `cp file1 file2` → Copy file  

\- `mv file1 file2` → Move/rename file  

\- `rm file` → Remove file  

\- `mkdir <dir>` → Create new directory  

\- `rmdir <dir>` → Remove empty directory  

\- `cat file` → Show file contents  

\- `nano file` → Edit file in nano editor  

\- `chmod 755 file` → Change file permissions  

\- `chown user:user file` → Change file owner  



---



\## 🔹 Networking Basics

\- `ifconfig` → Show network interfaces \& IP addresses  

\- `ip addr` → Modern alternative to ifconfig  

\- `ping <IP>` → Test connectivity  

\- `traceroute <IP>` → Show path packets take  

\- `netstat -tulnp` → List listening services/ports  

\- `ss -tulnp` → Modern netstat replacement  

\- `curl http://site.com` → Fetch webpage from CLI  



---



\## 🔹 Reconnaissance

\- `whois domain.com` → Get domain registration info  

\- `nslookup domain.com` → DNS lookup  

\- `dig domain.com` → Advanced DNS lookup  

\- `host domain.com` → Simple DNS resolver  



---



\## 🔹 Scanning with Nmap

\- `nmap <IP>` → Basic scan  

\- `nmap -sS <IP>` → Stealth TCP scan (SYN scan)  

\- `nmap -sU <IP>` → UDP scan  

\- `nmap -sV <IP>` → Detect service versions  

\- `nmap -O <IP>` → Detect operating system  

\- `nmap -A <IP>` → Aggressive scan (OS, version, scripts, traceroute)  

\- `nmap -p 1-65535 <IP>` → Full port scan  



---



\## 🔹 Wireshark Filters

\- `icmp` → Show only ICMP traffic (pings)  

\- `http` → Show HTTP traffic  

\- `ftp` → Show FTP traffic  

\- `dns` → Show DNS queries  

\- `tcp.port == 80` → Show traffic on port 80  

\- `ip.addr == 192.168.1.10` → Filter traffic for a specific host  



---



\## 🔹 Firewall (iptables)

\- `sudo iptables -L` → List rules  

\- `sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT` → Allow SSH  

\- `sudo iptables -A INPUT -p tcp --dport 80 -j DROP` → Block HTTP  

\- `sudo iptables -F` → Flush all rules  



---



\## 🔹 Useful Shortcuts

\- `Ctrl + C` → Stop process  

\- `Ctrl + Z` → Suspend process  

\- `fg` → Resume process in foreground  

\- `bg` → Resume process in background  

\- `history` → Show command history  

\- `!!` → Run last command again  



