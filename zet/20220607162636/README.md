# Inodes Can Store Data

While learning about inodes I came across something interesting. Inodes
can store data! If a small file is created the data is stored in the
inode. When the file reaches a certain size and the inode can no longer
hold the data a new block is assigned and the data is stored in the new
block. This also increases lookup time because the disk does not need to
be accessed to pull the data.

From what I have read there are two locations inodes have to store data.
The first is the inode.i_block and second is the ibody EA(extended
attributes). If the data is smaller than 60 bytes then the data is
stored in the i_bock. If over 60 bytes and the rest of the data can fit
into the ibody EA then the rest of the data is stored there. This would
give 160 bytes (in a 256 byte inode) of storage. That a lot!

This is very interesting to me. I have quite a few ideas and questions
that pop into my head.  
Does a virus or malware scanner scan inodes?  
Can you could store malicious scripts or code into a inode?  
Can you have multiple scripts stored that reference each other in inodes?  
Can you break down a larger malicious script into smaller blocks of code
and store them into inodes?  

Can I use the i_block of another file to store data? This question is
really interesting to me. Take the ping command. Ping is well over 60
bytes. Is the i_block being used? If not can I hide data in the i_block
of ping? Hmmmm.

Guess Ill do more research!

[https://ext4.wiki.kernel.org/index.php/Ext4_Disk_Layout#Inline_Data](https://ext4.wiki.kernel.org/index.php/Ext4_Disk_Layout#Inline_Data)

    #inodes #ext4 #linux #filesystem #learning
