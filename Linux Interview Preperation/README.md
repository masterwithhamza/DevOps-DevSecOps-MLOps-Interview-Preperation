
# Linux Interview Preperation 

### 1. What is Linux?
Linux is a free, open-source operating system based on Unix. It was created
by Linus Torvalds in 1991 and is widely used in servers, desktops, and embedded
systems.

#### Command: uname -a (displays system information)

### 2. What is the Linux kernel?
The Linux kernel is the core part of the Linux operating system that manages
hardware resources and provides essential services to other software.

#### Command: uname -r (displays kernel version)


### 3. Explain the directory structure in Linux.
The Linux directory structure follows a hierarchical format with root (/) at the
base. Important directories include /bin (binary executables), /etc (configuration
files), /home (user home directories), /var (variable data files), /usr (user programs),
and /tmp (temporary files).

#### Command: ls /

### 4. How do you check the current working directory?
You can check the current working directory using the pwd (print working
directory) command.
#### Command: pwd

### 5. How do you list files in a directory?
The ls command lists files in a directory. Adding options like -l provides a
detailed list, and -a includes hidden files.

#### Command: ls -la

### 6. How do you change file permissions?
The chmod command changes file permissions. Use symbolic (e.g., chmod
u+x file) or numeric (e.g., chmod 755 file) modes.

#### Command: chmod 755 filename

The chown command changes file ownership. The format is chown
owner:group filename.

#### Command: chown user:group filename

### 8. What is the purpose of the sudo command?
The sudo command allows a permitted user to execute a command as the
superuser or another user, as specified by the security policy.

#### Command: sudo command

### 9. How do you view the contents of a file?
You can use commands like cat, more, less, head, and tail to view file
contents.
#### Command: cat filename, less filename, head filename

### 10. How do you search for a file in Linux?
The find command searches for files in a directory hierarchy
#### Command: find /path -name filename

### 11. What is the difference between grep and egrep?
grep searches for patterns in files, while egrep (extended grep) supports
extended regular expressions.
#### Command: grep pattern filename, egrep pattern filename

### 12. How do you compress files in Linux?
Use commands like gzip, bzip2, and zip to compress files.
#### Command: gzip filename, zip archive.zip filename

### 13. How do you uncompress files in Linux?
Use commands like gunzip, bunzip2, and unzip to uncompress files.
#### Command: gunzip filename.gz, unzip archive.zip

### 14. What is a symbolic link?
A symbolic link is a file that points to another file or directory. It’s created
using the ln -s command.
#### Command: ln -s target linkname

### 15. How do you display disk usage?
The df command displays disk space usage, and du shows disk usage of
files and directories.
#### Command: df -h, du -sh directory

### 16. How do you check memory usage?
The free command displays memory usage, and top provides a dynamic
view of system processes and memory usage.
#### Command: free -h, top

### 17. What is a process in Linux?
A process is an instance of a running program. Linux manages processes
through process IDs (PIDs).
#### Command: ps, top

### 18. How do you list running processes?
The ps command lists running processes. Use ps aux for a detailed list.
#### Command: ps aux

### 19. How do you terminate a process?
Use the kill command followed by the process ID (PID). kill -9
PID forcefully terminates a process.
#### Command: kill PID, kill -9 PID

### 20. How do you change the priority of a process?
The nice command starts a process with a specified priority,
and renice changes the priority of an existing process.
#### Command: nice -n priority command, renice priority PID

### 21. What is a daemon in Linux?
A daemon is a background process that runs continuously and performs
specific operations, often started at boot time.

#### Example Daemon: sshd (Secure Shell Daemon)


### 22. How do you check open ports on a system?
The netstat and ss commands display network connections and listening
ports.
#### Command: netstat -tuln, ss -tuln


### 23. How do you set environment variables?
Use the export command to set environment variables.
#### Command: export VAR=value


### 24. How do you view environment variables?
The printenv or env commands display environment variables.
#### Command: printenv, env

### 25. How do you schedule tasks in Linux?
Use cron for scheduling recurring tasks and at for one-time tasks.
#### Command: crontab -e, at time

### 26. What is the difference between cron and anacron?
cron schedules tasks based on precise times, while anacron is used for
periodic tasks that are not time-sensitive and can run at any time after a system is
back online.
#### Command: crontab -e, anacrontab

### 27. How do you display the last login information?
The last command displays the last login information for users.
#### Command: last

### 28. How do you find the location of an executable?
Use the which command to find the location of an executable in the
system’s PATH.

#### Command: which executable

### 29. How do you count the number of lines, words, and characters in a file?
The wc command counts lines, words, and characters in a file.
#### Command: wc filename

### 30. How do you display the first and last few lines of a file?
Use the head command to display the first few lines and the tail command
to display the last few lines of a file.
#### Command: head filename, tail filename

### 31. How do you create a new user in Linux?
The useradd command creates a new user.
#### Command: sudo useradd username

### 32. How do you delete a user in Linux?
The userdel command deletes a user.
#### Command: sudo userdel username

### 33. How do you add a user to a group?
The usermod -aG command adds a user to a group.
#### Command: sudo usermod -aG groupname username

### 34. How do you switch users in Linux?
Use the su command to switch users.
#### Command: su - username

### 35. What is a shell in Linux?
A shell is a command-line interpreter that provides a user interface for the
Linux operating system. Examples include bash, sh, zsh, and csh.
#### Command: echo $SHELL

### 36. How do you check the Linux version?
The uname -a command displays system information, including the kernel
version. For distribution-specific information, use lsb_release -a.
#### Command: uname -a, `lsb_release -a

### 37. What is the /etc/passwd file?
The /etc/passwd file contains user account information, including
usernames, encrypted passwords, user IDs (UIDs), group IDs (GIDs), user info, home
directories, and default shells.
#### Command: cat /etc/passwd

### 38. What is the /etc/shadow file?
The /etc/shadow file stores encrypted user password information and
other password-related settings.
#### Command: cat /etc/shadow

### 39. How do you change your password in Linux?
Use the passwd command to change your password.
#### Command: passwd

### 40. What is the purpose of the /etc/fstab file?
The /etc/fstab file contains information about disk drives and partitions
that need to be mounted at boot time.
#### Command: cat /etc/fstab

### 41. How do you mount a filesystem?
Use the mount command to mount a filesystem.
#### Command: mount /dev/device /mnt

### 42. How do you unmount a filesystem?
Use the umount command to unmount a filesystem.
#### Command: umount /mnt

### 43. What is swap space?
Swap space is a portion of a hard disk used as virtual memory to
supplement physical RAM. It helps in managing memory when the system runs out of
RAM.
#### Command: swapon -s

### 44. How do you create a swap file?
You can create a swap file using the following commands :
#### Command: dd if=/dev/zero of=/swapfile bs=1M count=1024

### 45. How do you make a swap file permanent?
Add an entry to the /etc/fstab file
#### Command: echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab

### 46. What is the tar command used for?
The tar command is used to archive files. It can create, extract, and list the
contents of archives.
#### Command: tar -cvf archive.tar directory, tar -xvf archive.tar

### 47. How do you search for a pattern in a file?
The grep command searches for patterns within files.
#### Command: grep pattern filename

### 48. How do you copy files and directories?
Use the cp command to copy files and directories.
#### Command: cp source destination, cp -r source_directory destination_directory

### 49. How do you move or rename files and directories?
Use the mv command to move or rename files and directories.
#### Command: mv source destination

### 50. How do you delete files and directories?
Use the rm command to delete files and directories.
#### Command: rm filename, rm -r directory

### 51. What is the echo command used for?
The echo command outputs the given text or variables to the terminal.
#### Command: echo "Hello, World!"

### 52. How do you display a file's content in reverse order?
The tac command displays a file's content in reverse order.
#### Command: tac filename


### 53. How do you display a file's content in hexadecimal?
Use the xxd command to display a file's content in hexadecimal.
#### Command: xxd filename

### 54. What is the awk command used for?
The awk command is a powerful text processing utility used for pattern
scanning and processing.
#### 55. Command: awk '{print $1}' filename

### 56. What is the sed command used for?
The sed command is a stream editor used to perform basic text
transformations on an input stream.
#### Command: sed 's/old/new/' filename

### 56. How do you create an alias in Linux?
Use the alias command to create a shortcut for a command.
#### Command: alias ll='ls -la'

### 57. How do you remove an alias in Linux?
Use the unalias command to remove an alias.
#### Command: unalias alias_name

### 58. How do you create a hard link?
Use the ln command to create a hard link
#### Command: ln target linkname

### 59. What is the nohup command used for?
The nohup command allows a process to continue running in the
background after the user has logged out.
#### Command: nohup command &

### 60. How do you display the manual of a command?
Use the man command to display the manual of a command.
#### Command: man command

### 61. How do you display the help information of a command?
Use the --help option with the command to display its help information.
#### Command: command --help

### 62. What is a package manager?
A package manager is a tool that automates the process of installing,
upgrading, configuring, and removing software packages. Examples include apt, yum,
and dnf.
#### Command: apt-get install package, yum install package

### 63. How do you update a package list in Debian-based systems?
Use the apt-get update command to update the package list.
#### Command: sudo apt-get update

### 64. How do you upgrade all packages in Debian-based systems?
Use the apt-get upgrade command to upgrade all packages.
#### Command: sudo apt-get upgrade

### 65. How do you install a package in Debian-based systems?
Use the apt-get install command to install a package.
#### Command: sudo apt-get install package_name

### 66. How do you remove a package in Debian-based systems?
Use the apt-get remove command to remove a package.
#### Command: sudo apt-get remove package_name

### 67. How do you install a package in Red Hat-based systems?
Use the yum install or dnf install command to install a package.
#### Command: sudo yum install package_name, sudo dnf install package_name

### 68. How do you remove a package in Red Hat-based systems?
Use the yum remove or dnf remove command to remove a package.
#### Command: sudo yum remove package_name, sudo dnf remove package_name

### 69. How do you list installed packages?
Use the dpkg -l command in Debian-based systems and rpm -qa in Red
Hat-based systems.
#### Command: dpkg -l, rpm -qa

### 70. How do you check the dependencies of a package?
Use the apt-cache depends command in Debian-based systems and yum
deplist in Red Hat-based systems.
#### Command: apt-cache depends package_name, yum deplist package_name

### 71. How do you clean up unused packages?
Use the apt-get autoremove command in Debian-based systems and yum
autoremove in Red Hat-based systems to remove unused packages and
dependencies.
#### Command: sudo apt-get autoremove, sudo yum autoremove

### 72. What is the purpose of the /etc/hosts file?
The /etc/hosts file maps hostnames to IP addresses locally, allowing for
hostname resolution without querying DNS servers.
#### Command: cat /etc/hosts

### 73. Command: cat /etc/hosts?
Use commands like ifconfig (older systems) or ip (newer systems) to
configure network interfaces.
#### Command: ifconfig eth0 192.168.1.100 netmask 255.255.255.0

### 74. How do you check network configuration?
Use the ifconfig or ip addr command to check network configurations.
#### Command: ifconfig, ip addr

### 75. How do you check active network connections?
Use the netstat or ss command to check active network connections.
#### Command: netstat -tuln, ss -tuln

### 76. How do you restart a network service?
Use service management commands like systemctl or service to restart
network services.
#### Command: sudo systemctl restart network.service, sudo service network restart

### 77. What is the iptables command used for?
The iptables command is used to set up, maintain, and inspect the tables
of IP packet filter rules in the Linux kernel.
#### Command: sudo iptables -L

### 78. How do you enable packet forwarding?
Modify the /proc/sys/net/ipv4/ip_forward file to enable packet
forwarding.
#### Command: echo 1 | sudo tee /proc/sys/net/ipv4/ip_forward

### 79. What is a firewall in Linux?
A firewall in Linux is a system that controls incoming and outgoing network
traffic based on predetermined security rules. iptables and firewalld are common
firewall tools.
#### Command: sudo iptables -L, sudo firewall-cmd --state

### 80. How do you set up a simple firewall rule to block an IP address?
Use iptables to add a rule that blocks an IP address.
#### Command: sudo iptables -A INPUT -s 192.168.1.100 -j DROP

### 81. What is SELinux?
SELinux (Security-Enhanced Linux) is a Linux kernel security module that
provides a mechanism for supporting access control security policies.
#### Command: getenforce (to check the status), setenforce (to change the mode)

### 82. How do you disable SELinux temporarily?
 Use the setenforce command to change SELinux to permissive mode.
#### Command: sudo setenforce 0

### 83. What is the purpose of the /etc/resolv.conf file?
The /etc/resolv.conf file specifies the DNS servers that the system
should use for hostname resolution.
#### 84. Command: cat /etc/resolv.conf

### 85. How do you configure DNS settings?
Edit the /etc/resolv.conf file to configure DNS settings.
#### Command: sudo nano /etc/resolv.conf and add nameserver entries.

### 86. What is the hostname command used for?
The hostname command is used to display or set the system's hostname.
#### Command: hostname, sudo hostname newhostname

### 87. What is the scp command used for?
The scp (secure copy) command is used to securely copy files between
hosts over a network.
#### Command: scp file user@remote_host:/path/to/destination

### 88. How do you create an SSH key pair?
Use the ssh-keygen command to create an SSH key pair
#### Command: ssh-keygen -t rsa -b 2048

### 89. How do you add your SSH key to the SSH agent?
Use the ssh-add command to add your SSH key to the SSH agent.
#### Command: ssh-add ~/.ssh/id_rsa

### 90. What is the rsync command used for?
The rsync command is used for fast, flexible, remote (and local) file copying
and synchronization.
#### Command: rsync -avz source destination

### 91. How do you check the status of a service?
Use the systemctl or service command to check the status of a service.
#### Command: sudo systemctl status servicename, sudo service servicename status

### 92. How do you start and stop services?
Use the systemctl or service command to start and stop services.
#### Command: sudo systemctl start servicename, sudo systemctl stop servicename

### 93. What is a runlevel in Linux?
A runlevel is a mode of operation in Unix and Unix-like operating systems
that defines what system services are operating.
#### Command: runlevel

### 94. How do you change the runlevel?
Use the init or telinit command to change the runlevel.
#### Command: sudo init 3

### 95. What is the journalctl command used for?
The journalctl command is used to query and display messages from the
journal, which is the systemd logging service.
#### Command: journalctl

### 96. How do you enable and disable services at boot?
Use the systemctl command to enable or disable services at boot.
#### Command: sudo systemctl enable servicename, sudo systemctl disable servicename

### 97. What is two types of Linux User Mode ?
Command Line
GUI 

### 98. What is command for created multiple files at a time?
touch

### 99. What is INODE and How to Identify?
Its unique identification code for files and directories, its was generate automatically while create new file
and directories
ls -i filename
ls -ldi directoryname

### 100. List of Permissions and Users
Read, Write and Execute
Owner, Group Owners and Others

### List of Special Permissions and numerical value.
Set User ID = 4
Set Group ID = 2
Stickybit = 1



#
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hamzarehman4/)






## Authors

- [@hamza rehman](https://www.linkedin.com/in/hamzarehman4/)


## 🚀 About Me
My name is Hamza Rehman. I'm a passionate DevOps and MLOps enthusiast. With a deep interest in open-source technologies and automation,i enjoys sharing my knowledge and insights with the community.

