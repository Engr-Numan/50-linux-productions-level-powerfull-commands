# 50-linux-productions-level-powerfull-commands
50 linux productions level powerfull commands. these commands are very usefull in real environment in devops, sysops, linux-administrator roles, and in shell scripting 






Linux Powerfull Commands:::::::::::::::::::


50 Linux commands that are very useful for DevOps
tasks, along with brief explanations and examples:

1. rsync - Remote File Copy:
 - Efficiently copy files between local and remote systems.
# rsync -avz /local/path user@remote:/remote/path

2. awk - Text Processing:
 - A powerful text processing tool for pattern scanning and
reporting.

#cat logfile | awk '/error/ {print $1, $2}'

3. sed - Stream Editor:
 - Perform text transformations on input streams.


#cat file.txt | sed 's/old/new/g'
4. find - Search for Files:
 - Search for files in a directory hierarchy.

# find /path/to/search -name "*.txt"
5. tar - Archive and Compress:
 - Create compressed archive files.

# tar -czvf archive.tar.gz /path/to/directory

6. curl - Transfer Data with URLs:
 - Transfer data from or to a server.

# curl -O https://example.com/file.txt

7. lsof - List Open Files:
 - List information about files opened by processes.
# lsof -i :80

8. iptables - IP Packet Filter:
 - Configure IP packet filter rules.

# iptables -A INPUT -p tcp --dport 22 -j ACCEPT

9. grep - Search Text Patterns:
 - Search for patterns in files.
# grep "pattern" /path/to/search

10. awk '{print $NF}' - Extract Last Column:
 - Extract and print the last column from a file.
# cat data.txt | awk '{print $NF}'
11. tee - Redirect Output to File and Terminal:
 - Redirect output to a file and display it on the terminal.

# command | tee output.txt
12. htop - Interactive Process Viewer:
 - Display an interactive process viewer.

# Htop

13. netstat - Network Statistics:
 - Display network connections, routing tables, interface
statistics, masquerade connections, etc.

# netstat -tulpn

14. awk '!seen[$0]++' - Remove Duplicate Lines:
 - Remove duplicate lines from a file.
# awk '!seen[$0]++' file.txt

15. tail -n 20 - Display Last 20 Lines:
 - Display the last N lines of a file.
# tail -n 20 logfile.txt
16. du -h - Show Disk Usage:
 
 - Display disk usage of files and directories.

# du -h /path/to/directory

17. ps aux | grep process_name - List Processes:
 - List all processes and filter by name.

# ps aux | grep nginx

18. watch -n 1 command - Execute Command Periodically:
 - Run a command repeatedly at a specified interval.

# watch -n 1 "ps aux | grep process_name"

19. df -h - Display Free Disk Space:
 - Show free disk space on mounted filesystems.

# df -h

20. nc -l 8080 - Simple Netcat Server:
 - Start a simple server using netcat.

# nc -l 8080

21. cut -d' ' -f1 - Extract First Column:
 - Extract and print the first column from a file.
# cut -d' ' -f1 file.txt

22. journalctl - View System Logs:
 - Query and display messages from the journal.
# journalctl -xe

23. chmod +x filename - Make File Executable:
 - Grant execute permission to a file.

#chmod +x script.sh

24. chown user:group filename - Change File Owner:
 - Change the owner and group of a file.
# chown user:group file.txt
25. nohup command & - Run Command in Background:
 - Run a command that keeps running even after logging
out.
# nohup ./script.sh &

26. head -n 10 - Display First 10 Lines:
 - Display the first N lines of a file.
# head -n 10 file.txt

27. fdisk -l - List Partitions:
 - Display the partition table for all disks.
# fdisk -l

28. history - View Command History:
 - Display the command history for the current session.

# History

29. uptime - Check System Uptime:
 - Display how long the system has been running.
# Uptime

30. crontab -e - Edit Cron Jobs:
 - Edit the crontab file to schedule jobs.

# crontab -e

31. ip a - Show IP Addresses:
 - Display network interfaces and their IP addresses.

# ip a

32. systemctl status service_name - Check Service Status:
 - View the status of a systemd service.

# systemctl status ssh
33. echo "Hello, World!" > file.txt - Write to File:
 - Write text to a file (overwrites existing content).
# echo "New content" > file.txt

34. useradd username - Add User:
 - Add a new user to the system.

# useradd john_doe

35. passwd username - Set User Password:
 - Set or change the password for a user.

# passwd john_doe

36. ps -ef - Show All Processes:
 - Display information about all processes.

# ps -ef

37. kill -9 process_id - Forcefully Kill Process:
 - Terminate a process forcefully.

# kill -9 12345

38. scp file.txt user@remote:/path - Secure Copy:
 - Copy files securely between local and remote systems.

#scp localfile.txt user@remote:/path

39. free -m - Display Free Memory:
 - Show the amount of free and used memory.
# free -m
40. systemctl restart service_name - Restart Service:
 - Restart a systemd service.

# systemctl restart apache2

41. echo $VARIABLE - Display Environment Variable:
 - Display the value of an environment variable.
# echo $HOME

42. ps aux | sort -rk 3,3 - Top CPU Consuming Processes:
 - List processes sorted by CPU usage.

# ps aux | sort -rk 3,3

43. tail -f /var/log/auth.log - Monitor Authentication Logs:
 - Continuously monitor authentication logs.

# tail -f /var/log/auth.log

44. systemctl stop service_name - Stop Service:
 - Stop a systemd service.

# systemctl stop nginx

45. wget - Download Files from the Web:
 - Download files from the internet.

# wget https://example.com/file.txt

46. grep -i "error" /path/to/log/*.log - Case-Insensitive
Search:
 - Search for errors in logs regardless of case.


# grep -i "error" /path/to/log/*.log

47. df -Th - Display Disk Space Usage with Type:
 - Show disk space usage with filesystem type.


# df -Th

48. journalctl --since "2023-01-01" - View Logs Since Date:
 - Display journal logs since a specific date.

# journalctl --since "2023-01-01"


49. systemctl enable service_name - Enable Service at Boot:
 - Enable a systemd service to start at boot.

# systemctl enable apache2

50. awk -F: '/\/home/ {print $1, $7}' /etc/passwd - Extract

User and Home Directory:
 - Extract and print username and home directory from
/etc/passwd.

# awk -F: '/\/home/ {print $1, $7}' /etc/passwd
