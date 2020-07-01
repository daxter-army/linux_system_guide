# ls command options

* **ls** *-a* - This will list all the files in your current working directories including hidden files that start with .

* **ls** *-l* - That's a **long listing** that we saw before, It shows many impotant information about a file. Permssions, Number of Links, Owner, Group, File size, Modification Date, File name

* **ls** *-t* - This will list the files sorted by modification date. Newest first

* **ls** *-r* - This will list the files in reversed fashion

* **ls** *-i* - This will list the *index node* number of each file in the current working directory


## The recursive option

* **ls** *-R* - So if you want to list the contents of a directory and all it's subdirectories you use

* For example, Imagine if you have a directory named dir1 on your desktop, and inside dir1 you have a subdirectory named dir2. Now, if you type ls ­R dir1, Then this will list the contents of
dir1 and dir2.

* Notice that if dir2 has another subdirectory dir3 then **ls ­R** dir1 will also list the files of dir3 and so on ... got it now ?

* Here comes the interesting part, if you executed **ls ­R /** then this will list all the files (non hidden) on your system


## Combinig command options

* **ls** *-R* *-a* - list all the files including hidden files on your system | or **ls** *-Ra*

* You can also write it as **ls -a -R** or **ls -aR**, order doesn't matter

* **ls** *-Ra /* - will list all files on your system

* **ls** *­-latR /* - will make a long listing of all the files on your system sorted by modification date (newest first)

* Command options are case sensitive -R (Recursive) is not same as -r (reverse listing)

* If you want to list the files in reverse order based on time then we can combine *-­r* & *-­t* so , ls *-­tr* will list the files sorted by modification date (Oldest first)
