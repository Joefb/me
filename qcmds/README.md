# Quick Commands
This repo is a list of commands that I forget all the time or new ones 
I have learned about.
---
### Python
* `python3 -m http.server 8000` - Python 3 simple server 

### Shell Commands
* `source ~/.bashrc` - Reload bashrc 
* `df -h` - Display file system disk space uasge 
* `ln -s item link` - Create sym link 
* `stat fileName` - Shows stats of a file or file system
* `sync` - Forces all data in cache to be written to disk
* `whatis` - Display one-line man page description
* `type` - Indicate how the cmd is interpreted
* `which` - Display which exe program will be excuted
* `apropos` - search the manual page names and descriptions
* `info` - Display cmds into entry
* `alias` - Create an alias for a command or commands
* `zless` - Display the contents of gzip compressed txt files

### Apt commands
* `apt update` - Updates the list of available packages and their versions
* `apt install` - Install a package and its dependencys
* `apt purge` - Removes a package and its config files
* `apt remove` - Removes a package and will NOT remove the config files
* `apt autoremove` - Removes all unused packages
* `apt autoremove --purge` Removes all unused packages and their cfg files
* `apptitude why pkgName` Shows info on why a package installed 
* `apt-cache show pkgName` Shows detailed info about a package

### Dpkg commands
* `dpkg -l | grep pkgName` - Search installed packages
* `dpkg -L pkgName` - Shows what a package has installed 
* `dpkg -S fileName` - Show what package provides the file

