# My Bash Notes

Wildcards:</br>
* `*` Matches any char
* `?` Matches any single char
* `[chars]` Matches any char that is a member of the set chars
* `[!chars]` Matches any char that is not a member of the set chars
* `[[:class:]]` Matches any char that is a member of the specified class

Commonly Used Char Classes:</br>
* `[:alnum:]` Matches any alphanumeric char
* `[:alpha:]` Matches any alphabetic char
* `[:digit:]` Matches any numeral 
* `[:lower:]` Matches any lowercase letter
* `[:upper:]` Matches any uppercase letter

Commonly used ls options:</br>
* `-A` List all files except . and ..
* `-F` Append indicator char at the end of each file
* `-h` Display file sizes in human readable format
* `-r` List files in reverse order
* `-S` Sort by file size
* `-t` Sort by modification time

Commonly used cp options:</br>
* `-a` Copy files and dirs and all attributes, ownerships and permissions
* `-i` Prompt before overwriting files
* `-u` Only copy files that dont exist or are newer
* `-v` Verbose mode

Commonly used mv options:</br>
* `-i` Prompt before overwriting files
* `-u` Only copy files that dont exist or are newer
* `-v` Verbose mode

Commonly used rm options:</br>
* `-i` Prompt before overwriting files
* `-u` Only copy files that dont exist or are newer
* `-v` Verbose mode
* `-f` Ignore nonexistent files and do not prompt

`cp dir1/*` Will copy all files in dir1

*Useful tip:* When using rm with wildcards, test the wildcard first with
ls to see what files will be deleted.

