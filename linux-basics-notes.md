Beginner-friendly notes for cybersecurity and SOC learning

## 📁 1. Linux Directory Structure (Most Important Paths)
Path	Purpose
/	Root directory (top of filesystem)
/home/	User home folders
/var/log/	All logs stored here
/etc/	System configuration files
/usr/bin/	User commands & binaries
/opt/	Optional/3rd-party software
/tmp/	Temporary files

## 📌 2. Basic File & Directory Commands
Navigation
ls
ls -l
cd foldername
pwd
File operations
touch file.txt
cat file.txt
cp file.txt backup.txt
mv file.txt newname.txt
rm file.txt
Directory operations
mkdir testfolder
rmdir emptyfolder
rm -r foldername

## 📌 3. Viewing File Content
cat filename
less filename
head filename
tail filename
tail -f /var/log/auth.log

## 📌 4. Users & Permissions
Check file permissions
ls -l
Change file permissions
chmod 755 file
chmod u+rwx file
chmod g-w file
Change ownership
sudo chown user:group file
User & group commands
sudo adduser username
sudo deluser username
groups username
id username

## 📌 5. Processes & System Monitoring
List running processes
ps aux
top
htop
Kill a process
kill PID
kill -9 PID
Service control
systemctl status apache2
systemctl start apache2
systemctl stop apache2

## 📌 6. Network Commands
ip a
ifconfig
ping google.com
traceroute google.com
curl example.com
wget example.com/file
nslookup domain.com
dig domain.com
Check open ports
ss -tuln
netstat -tulnp

## 📌 7. Important Log Files
Log File	Description
/var/log/syslog	System activity
/var/log/auth.log	Authentication events
/var/log/kern.log	Kernel logs
/var/log/dmesg	Hardware messages
Commands
journalctl
grep "Failed" /var/log/auth.log
grep "error" /var/log/syslog

## 📌 8. Basic Bash Scripting
Example script:

#!/bin/bash
echo "Hello, this is my first script"

Make executable:
chmod +x script.sh
./script.sh
