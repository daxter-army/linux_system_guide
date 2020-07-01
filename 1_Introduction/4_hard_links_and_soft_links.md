# Linux Links

## Inode

* Every file in the system has an inode (Index Node)
* It contains all file information except the file contents and name
* It's just like a personal ID or a passport (Without a name!)

## They contains the the following info;

* Inode Number
* File Size
* Owner Info
* Permissions
* File Type
* Number of links etc

Here, we will discuss about **Links**

* There are 2 types of links
	> Soft Links
	> Hard Links

### Soft Links

* a.k.a. Symbolic Links
* as we all know, it is a pointer to the original file
* we can see it just like a *shortcut* in windows
* generally, is of smaller size than the original file
* a soft link has a different inode number than the original file
* it is also clear that, if we delete the original file, **shortcut** will become useless

### Hard Links

* It is different name of the same file
* has same file size as that of original
* same inode number as that of original file, as like a shortcut with exact same file size and same **inode number**
* we **can't differentiate between a hard link and an original file**
* it's like a copy of the original file, if we delete the original, this will not affect our hard link file by any means
