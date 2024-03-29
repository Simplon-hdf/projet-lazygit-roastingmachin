# cheatsheet terminal

### File System Navigation  
- `ls` Lists files and directories in the current directory.
- `cd [directory_name]` Changes the working directory.
- `pwd` Prints the path of the current directory.
- `cat [file_name]` Display file contents.
- `less [file_name]` View file contents one page at a time.
- `head [file_name]` Display the first few lines of a file.
- `tail [file_name]` Display the last few lines of a file.
- `grep [pattern] [file_name]` Search for a pattern in a file.

### File Manipulation

- `touch [file_name]` Creates a new empty file.
- `nano [file_name]` Opens the file in the Nano text editor.
- `mkdir [directory_name]` Creates a new directory.
- `rm [file_name]` Deletes a file.
    - `-rf ` Deletes all child of this file or directory
- `rmdir [directory_name]` Deletes an empty directory.
- `cp [source] [destination]` Copies files or directories.
- `mv [source] [destination]` Moves or renames files or directories.

### Permission Management

- `chmod [permissions] [file_name]` Changes the permissions of a file or directory.
    - `-R` Recursively change permissions of directories and their contents.
- `chown [user:group] [file_name]` Changes the owner and/or group of a  file or directory.
    - `-R` Recursively change ownership of directories and their contents.
- `chgrp group file/directory` This command is used to change the group ownership of a file or directory.  
    - `-R` Recursively change group ownership of directories and their contents.
### Processes and System

- `ps` Displays active processes.
    - `-e` Display information about all processes.
    - `-f` Display a full listing.
    - `-u user` Display processes owned by a specific user.
    - `aux` Display a detailed listing of all processes.
- `kill [PID]` Kills a process using its Process ID (PID).
- `top` Displays running processes and their resources.
    - `q` Quit top.
    - `k` Kill a process.
    - `u` Specify user.
    - `H` Toggle threads display.
    - `P` Sort by CPU usage.
    - `M` Sort by memory usage.
    - `R` Reverse the sorting order.

### Archives and Compression

- `tar -cvf [archive_name.tar] [files]` Creates a tar archive.
- `tar -xvf [archive_name.tar]` Extracts a tar archive.
- `gzip [file_name]` Compresses a file using gzip.
- `gunzip [file_name.gz]` Decompresses a gzip file.

### Networking

- `ping [ip_address_or_domain_name]` Checks network connectivity.
- `ifconfig` Displays information about network interfaces.
- `ssh [user@ip_address]` Connects to a remote machine via SSH.
    - `-p` Add a port to the adress
	- `-l` Login name
- `scp [file] [user@ip_address:destination]` Copies files via SSH.

Help and Documentation

- `man [command]` Displays the manual for a specific command.
    - `--help` Add this to a command to display quick help.