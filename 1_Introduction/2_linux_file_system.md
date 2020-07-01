# Linux File System Structure

* It has a tree like structure also known as *directory tree*.

* What we call **Folder** in *Windows*, are **Directory** in *Linux*, but these terms are quite often used interchangeably.

* **directory tree** is like a *family tree* but it has only one **Parent**.

* There is a **root directory** with no parent at all, it is the parent of all.

* Root Directory contains several other sub directories, some of them are; 

1. **bin** (a.k.a binary) - contains executables programs and commands that can be used by all the users on the system.

2. **opt** (a.k.a optional) - this contains all the commercial softwares that are not installed by deafult on your system.

3. **home** - each user is given a sub-directory, user related files are stored in their respective direcrories.

4. **tmp** (a.k.a temporary)- temporary files on your system, addition and substration of files is quite common and often there. **DO NOT KEEP YOUR FILES HERE, EVER. YOU WILL LOST THEM.**

5. **var** - it contains valuable data that gets frequently changed over time, contains log files, user databases, mail pools etc.

* current dir (denoted by **.**) - it denotes your current directory in which you are in at that time.

* parent dir (denoted by **..**) - it denotes parent directory to your current directory. helps in moving to parent dir from cli.

*both common to all directories, can be found in every directory*

# Paths

* For accessing a file we can use;
    1. absolute path
    2. relative path 

* Absolute path starts from root dir
> */home/daxter-army/documents/mail.md*

* Relative path starts from current dir, lets say your current dir is *./daxter-army*
> *./documents/mail.md*