# super-useful-Linux-commands-for-beginners
50+ super useful Linux commands for beginners

File & Directory Navigation

| Command | Description                                           |
| ------- | ----------------------------------------------------- |
| `ls`    | List files and directories                            |
| `ls -l` | Long listing (shows permissions, size, etc.)          |
| `ls -a` | Show hidden files                                     |
| `cd`    | Change directory                                      |
| `pwd`   | Show current working directory                        |
| `tree`  | Show directory structure as a tree (optional package) |
| `clear` | Clear the terminal screen                             |

File & Directory Management

| Command                | Description                      |
| ---------------------- | -------------------------------- |
| `touch file.txt`       | Create a new empty file          |
| `mkdir folder`         | Create a new directory           |
| `rm file.txt`          | Remove a file                    |
| `rm -r folder`         | Remove a folder and its contents |
| `cp file1 file2`       | Copy file1 to file2              |
| `mv file1 file2`       | Move or rename files             |
| `find . -name "*.txt"` | Find files with `.txt` extension |
| `stat file.txt`        | Show detailed file info          |

Viewing & Editing Files

| Command                   | Description                           |
| ------------------------- | ------------------------------------- |
| `cat file.txt`            | View file contents                    |
| `less file.txt`           | Scroll through file content           |
| `head file.txt`           | View first 10 lines                   |
| `tail file.txt`           | View last 10 lines                    |
| `nano file.txt`           | Edit file in a simple terminal editor |
| `vim file.txt`            | Edit file in advanced editor (vim)    |
| `echo "text" > file.txt`  | Write to a file (overwrite)           |
| `echo "more" >> file.txt` | Append text to a file                 |

System Info & Monitoring

| Command    | Description                                   |
| ---------- | --------------------------------------------- |
| `uname -a` | Full system info                              |
| `top`      | Live view of running processes                |
| `htop`     | Colorful process viewer (may need to install) |
| `df -h`    | Disk space usage                              |
| `free -h`  | Show memory usage                             |
| `uptime`   | System uptime                                 |
| `whoami`   | Show current user                             |
| `id`       | User and group IDs                            |
| `ps aux`   | Show all running processes                    |

Network Commands

| Command            | Description                |
| ------------------ | -------------------------- |
| `ping google.com`  | Check network connectivity |
| `ip a`             | Show network interfaces    |
| `netstat -tuln`    | Show open ports            |
| `curl ifconfig.me` | Show your public IP        |
| `hostname`         | Display system hostname    |

Package Management (Debian/Ubuntu)

| Command                    | Description                |
| -------------------------- | -------------------------- |
| `sudo apt update`          | Refresh package list       |
| `sudo apt upgrade`         | Upgrade installed packages |
| `sudo apt install package` | Install a new package      |
| `sudo apt remove package`  | Uninstall a package        |
| `dpkg -l`                  | List installed packages    |

Permissions & Ownership

| Command                 | Description                |
| ----------------------- | -------------------------- |
| `chmod +x file.sh`      | Make script executable     |
| `chmod 755 file`        | Set file permissions       |
| `chown user:group file` | Change ownership of a file |

user → The new owner of the file

group → The new group

file → The file or directory you're modifying

Example:

sudo chown alice:developers report.txt

Sets alice as the owner, and developers as the group of report.txt. 

Miscellaneous & Power Tools

| Command                   | Description                      |
| ------------------------- | -------------------------------- |
| `history`                 | Show command history             |
| `alias ll='ls -lah'`      | Create a shortcut command        |
| `man command`             | View manual/help for any command |
| `tar -xvzf file.tar.gz`   | Extract `.tar.gz` archive        |
| `zip -r file.zip folder/` | Create a zip archive             |
| `unzip file.zip`          | Extract zip archive              |
| `crontab -e`              | Edit scheduled tasks             |
| `sudo`                    | Run a command as root/superuser  |

Alias Example:

alias ping='ping -c4'

ping www.google.com (will ping 4 times only)

unalias ping (will remove the shortcut command)

alias (will show all alias shortcut commands)

Zip Example:

You are here: /home/debian/Desktop

You have a folder on Desktop called "auto" that contains 5 files.

To make a zip file of "auto" you have to type:

zip -r cars.zip auto/

zip: The command to create a ZIP archive.
-r: Stands for "recursive", meaning it will include all files and subdirectories inside auto/.
cars.zip: The name of the ZIP file you want to create.
auto/: The folder you want to compress.  
