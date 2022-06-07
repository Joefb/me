# The Linux File System.

## ext4 file system

**How Ext file system stores data:**</br>

**Superblock** - The first block on the file system that contains
information about the drive. Tells the kernel where everything is and
how to how to address it.

**Group Descriptor** - Describes groups of blocks of data on the drive

**Reserved Group Descriptor Blocks** - Used for extra copies of group
descriptors

**Block Bitmap** - A bit map that tells if the block is being used.

**Inode Bitmap** - A bit map that tells if the inode is being used.

**Inode Table** - Contains the information on files and where the files are
stored.

**Data Blocks** - Where the actual data in the files are stored.

**Example of the bit maps** - In the case of Inode bitmap table each inode
points to a bit in the bit map. If the bit is a 1 then that says that
the inode is being used. If the bit is a 0 then that says the inode is
not being used.

**Inside of an Inode**
* User and group owner IDs
* File type
* Permissions
* Data access and create time
* Inode modified time
* Number of hard links
* File size
* Pointers to the data in the data block

**ext4 inodes can hold data**
Inodes in ext4 can also hold the data of a file if the size is 60 bytes
or under.
[Link](https://ext4.wiki.kernel.org/index.php/Ext4_Disk_Layout#Inline_Data)

---

## File System Structure and Descriptions
*Taken from The Linux Command Line by William Shotts*

**/**</br>
The root directory. Where everything begins.

**/bin**</br>
Contains binaries (programs) that must be present for the
system to boot and run.

**/boot**</br>
Contains the Linux kernel, initial RAM disk image (for
drivers needed at boot time), and the boot loader.

**/dev**</br>
This is a special directory that contains device nodes.
“Everything is a file” also applies to devices. Here is where
the kernel maintains a list of all the devices it understands.

**/etc**</br>
The /etc directory contains all of the system-wide
configuration files. It also contains a collection of shell
scripts that start each of the system services at boot time.
Everything in this directory should be readable text.

**/home**</br>
In normal configurations, each user is given a directory in
/home. Ordinary users can only write files in their home
directories. This limitation protects the system from errant
user activity.

**/lib**</br>
Contains shared library files used by the core system
programs.

**/lost+found**</br>
Each formatted partition or device using a Linux file system,
such as ext4, will have this directory. It is used in the case of
a partial recovery from a file system corruption event.
Unless something really bad has happened to our system,
this directory will remain empty.

**/media**</br>
On modern Linux systems the /media directory will
contain the mount points for removable media such as USB
drives, CD-ROMs, etc. that are mounted automatically at
insertion.

**/mnt**</br>
On older Linux systems, the /mnt directory contains mount
points for removable devices that have been mounted
manually.

**/opt**</br>
The /opt directory is used to install “optional” software.
This is mainly used to hold commercial software products
that might be installed on the system.

**/proc**</br>
The /proc directory is special. It's not a real file system in
the sense of files stored on the hard drive. Rather, it is a
virtual file system maintained by the Linux kernel. The
“files” it contains are peepholes into the kernel itself. The
files are readable and will give us a picture of how the
kernel sees the computer.

**/root**</br>
This is the home directory for the root account.

**/sbin**</br>
This directory contains “system” binaries. These are
programs that perform vital system tasks that are generally
reserved for the superuser.

**/tmp**</br>
The /tmp directory is intended for the storage of temporary,
transient files created by various programs. Some
configurations cause this directory to be emptied each time
the system is rebooted.

**/usr**</br>
The /usr directory contains all the programs and support files used
by regular users.

**/usr/bin**</br>
The /usr/bin contains the executable programs installed by
the Linux distribution.

**/usr/lib**</br>
The shared libraries for the programs in /usr/bin.

**/usr/local**</br>
The /usr/local tree is where programs that are not
included with the distribution but are intended for system-
wide use are installed. Programs compiled from source code
are normally installed in /usr/local/bin.

**/usr/sbin**</br>
Contains more system administration programs.

**/usr/share**</br>
/usr/share contains all the shared data used by
programs in /usr/bin. This includes things such as
default configuration files, icons, screen backgrounds, sound
files, etc.

**/usr/share/doc**</br>
Most packages installed on the system will include some
kind of documentation. In /usr/share/doc, we will find
documentation files organized by package.

**/var**</br>
The /var directory tree is where data that is likely to change is stored.
Various databases, spool files, user mail, etc. are located here.

**/var/log**</br>
/var/log contains log files, records of various system
activity.
