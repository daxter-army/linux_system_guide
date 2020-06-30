# Basic Linux Commands
1. date
2. cal
3. cal -y
4. cal -3
5. cal <year>
6. cal <month_number> <year>
7. clear
8. exit

# Linux File Systems
* has a tree like structure aka directory tree
* folder in windows and directory in linux, but these terms are used quite often used interchangeably

* **directory tree** like family tree but have only only one parent
* there is a root folder with no parent at all, it is the parent for all.
* contains several other sub directories 
1. bin (binary) - containes executables programs and commands that can be used by all the users on the system
2. opt (optional) - this contains all the commercial softeares that are not installed by deafult on your system
3. home - each user is given a subdirectory, user related files are strored in their respective direcrories
4. tmp (temporary)- temporary files on your system, often deletes files in this
5. var - it contains valuable data that gets frequently changed over time, contains log files,user databases, mail pools
6. current dir (.)
7. parent dir (..)
both common to all directories, can be found anywhere

**access a file (absolute vs relative paths)**
1. /home/daxter-army/phone/mehul.txt (abs path starts from root dir)
2. ./documents/phone.txt (rel path starts from current dir)

**Navigation between directories**
1. pwd - print working directory - display absolute path of current working dir
2. ls - list diretory contents
* ls / - list contents of root dir
* ls ~ - list contents of home dir
* ls .. - list contents of parent dir
3. cd - change dir
4. cd / - go at root dir
5. cd ~ - go to home
6. cd .. - go to parent dir
7. cd - go to previous work dir

**Links**