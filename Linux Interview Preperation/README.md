
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

### 

####

###

####

###

####

###

####

###

####

###

####

###

####

###

####

###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####

###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####
###

####


#
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hamzarehman4/)






## Authors

- [@hamza rehman](https://www.linkedin.com/in/hamzarehman4/)


## 🚀 About Me
My name is Hamza Rehman. I'm a passionate DevOps and MLOps enthusiast. With a deep interest in open-source technologies and automation,i enjoys sharing my knowledge and insights with the community.

