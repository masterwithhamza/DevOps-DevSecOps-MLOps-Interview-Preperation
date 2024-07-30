
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

