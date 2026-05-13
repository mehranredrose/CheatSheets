# Terminal Commands Cheat Sheet

Terminal commands are essential for interacting with operating systems and managing files efficiently. Below is a detailed cheat sheet to help you get started with common terminal commands across Unix-like systems (Linux, macOS).

## Basic Navigation

### Change Directory
Change the current working directory.
```bash
cd path/to/directory
```

Example:
```bash
cd ~/Documents/
```

### List Directory Contents
List files and directories in the current directory.
```bash
ls
```

List all files including hidden ones.
```bash
ls -a
```

### Make a New Directory
Create a new directory.
```bash
mkdir new_directory
```

Example:
```bash
mkdir my_project
```

### Remove a Directory
Remove an empty directory.
```bash
rmdir empty_directory
```

Remove a directory with its contents recursively.
```bash
rm -r directory_with_contents
```

### Rename or Move a File/Directory
Rename a file or move it to another location.
```bash
mv old_name new_name
```

Example:
```bash
mv project.txt documents/project.txt
```

## File Operations

### Create a New File
Create an empty file.
```bash
touch filename
```

Example:
```bash
touch README.md
```

### Copy Files/Directories
Copy files or directories.
```bash
cp source destination
```

Example:
```bash
cp file.txt backup/
cp -r directory new_directory
```

### Move/Copy Files and Directories
Move or copy files and directories to a different location.
```bash
mv source destination
cp source destination
```

Example:
```bash
mv project.txt /home/user/projects/
cp documents/report.pdf /home/user/archive/
```

### Remove Files/Directories
Remove files.
```bash
rm filename
```

Example:
```bash
rm file.txt
```

Remove directories with their contents recursively.
```bash
rm -r directory_with_contents
```

Example:
```bash
rm -r my_old_project/
```

## Viewing and Editing Files

### View File Contents
View the contents of a file in the terminal.
```bash
cat filename
less filename
more filename
head filename
tail filename
```

Example:
```bash
cat README.md
less project.txt
head /etc/passwd
tail -n 10 /var/log/syslog
```

### Edit Files
Edit files using a text editor like `nano`, `vim`, or `emacs`.

**Using nano:**
```bash
nano filename
```

Example:
```bash
nano my_code.py
```

**Using vim:**
```bash
vim filename
```

Example:
```bash
vim README.md
```

**Using emacs:**
```bash
emacs filename
```

Example:
```bash
emacs project.txt
```

## Text Processing

### Search in Files
Search for text within files.
```bash
grep "search_term" filename
```

Example:
```bash
grep "hello world" README.md
```

### Count Lines, Words, and Characters
Count lines, words, and characters in a file.
```bash
wc -l filename
wc -w filename
wc -c filename
```

Example:
```bash
wc -l project.txt
wc -w /etc/passwd
wc -c README.md
```

## Compression and Archiving

### Compress Files
Compress files using gzip.
```bash
gzip filename
```

Example:
```bash
gzip file.txt
```

Decompress a `.gz` file.
```bash
gunzip filename.gz
```

Example:
```bash
gunzip file.txt.gz
```

### Create Tar Archives
Create a tar archive of multiple files or directories.
```bash
tar -cvf archive.tar directory/
```

Example:
```bash
tar -cvf my_project.tar my_project/
```

Extract a tar archive.
```bash
tar -xvf archive.tar
```

Example:
```bash
tar -xvf my_project.tar
```

### Compress with gzip and tar
Compress with gzip and tar.
```bash
tar -czvf archive.tar.gz directory/
```

Example:
```bash
tar -czvf my_project.tar.gz my_project/
```

Extract a `.tar.gz` file.
```bash
tar -xzvf archive.tar.gz
```

Example:
```bash
tar -xzvf my_project.tar.gz
```

## Permissions

### Change File Permissions
Change the permissions of a file or directory using `chmod`.
```bash
chmod mode filename
```

Mode can be specified in symbolic (e.g., `u+x`, `g-w`) or octal format.
Example:
```bash
chmod 755 script.sh
```

### Change Ownership
Change the ownership of a file or directory using `chown`.
```bash
chown user:group filename
```

Example:
```bash
chown john:developers report.pdf
```

## Networking

### Check Network Connectivity
Check network connectivity to a host.
```bash
ping hostname_or_ip
```

Example:
```bash
ping google.com
```

### View Network Interfaces
View information about network interfaces.
```bash
ifconfig
ip addr show
```

Example:
```bash
ifconfig eth0
ip addr show eth0
```

### Download Files
Download files from the web using `wget` or `curl`.
```bash
wget url
curl -O url
```

Example:
```bash
wget http://example.com/file.zip
curl -O https://example.com/data.json
```

## System Information

### Get System Uptime
Get the system uptime.
```bash
uptime
```

Example:
```bash
uptime
```

### View Disk Space Usage
View disk space usage with `df`.
```bash
df -h
```

Example:
```bash
df -h
```

### View Memory Usage
View memory usage with `free`.
```bash
free -m
```

Example:
```bash
free -m
```

### Get Process Information
Get process information using `ps` and `top`.
```bash
ps aux
top
```

Example:
```bash
ps aux | grep my_process
top
```

## Environment Variables

### Set an Environment Variable
Set an environment variable.
```bash
export VARIABLE_NAME=value
```

Example:
```bash
export PATH=$PATH:/home/user/bin
```

### List Environment Variables
List all environment variables.
```bash
env
printenv
```

Example:
```bash
env | grep HOME
printenv USER
```

## Shell Aliases

### Create a Shell Alias
Create a shell alias to simplify commands.
```bash
alias alias_name='command'
```

Example:
```bash
alias ll='ls -la'
```

### List Aliases
List all defined aliases.
```bash
alias
```

Example:
```bash
alias ll
```

## Miscellaneous

### Clear Terminal Screen
Clear the terminal screen.
```bash
clear
```

Example:
```bash
clear
```

### Exit Terminal
Exit the terminal session.
```bash
exit
```

Example:
```bash
exit
```

This cheat sheet provides a comprehensive overview of common terminal commands. By mastering these elements, you can efficiently manage your files and perform various tasks in the terminal.

Happy using the terminal!
```
You can save this content in a file named `terminal-commands.md` in your cheatsheets directory. Feel free to modify it further to suit your needs!
