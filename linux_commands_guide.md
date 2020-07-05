# Linux Commands

## Basic Commands
* **date** - prints current system date
* **cal** - prints current month
	* **cal** *-y* - prints current year
	* **cal** *-3* - prints previous, current & next months
	* **cal** *<specific_year>* - prints calender of specific year
	* **cal** *<month_number>* *<specific_year* - prints calender of specific month of specific year
* **clear** - clears the area
* **exit** - exit terminal

## Navigation between directories (ls & cd)
* **pwd** *(print working directory)* - display absolute path of current working dir
* **ls** - list diretory contents
	* **ls** */* - list contents of root dir
	* **ls** *~* - list contents of home dir
	* **ls** *..* - list contents of parent dir

* **cd** */* - go at root dir
	* **cd** *~* - go to home
	* **cd** *..* - go to parent dir
	* **cd** *-* go to previous work dir

## View Inode Numbers
* **ls** *-i* - show inode numbers of all files in current directory
	* **ls** *-i /* - show inode numbers of all files in root directory
	* **ls** *-l* - show additional info like file size (bytes), owner etc about files present in current dir

## Create Hard/Soft links
* **ln <file_name> <hardlink_name>** - create a hardlink of the desired file
	* **ln** *-s* **<file_name/dir_name> <softlink_name>** - create softlinks of the desired file

**NOTE - Hardlinks are not allowed for directories, they were allowed earlier, but they have been disabled now, because it was producing ambiguity in the file system**

## Create loops in directories
* **ln** *-s* *<abs_path>/<rel_path>/<..>* - create a loop using softlink

**NOTE - Because hardlinks are not allowed for directories, loops can't be created with hardlinks**

## ls command options
* **ls** *-a* - This will list all the files in your current working directories including hidden files that start with .
* **ls** *-l* - That's a **long listing** that we saw before, It shows many impotant information about a file. Permssions, Number of Links, Owner, Group, File size, Modification Date, File name
* **ls** *-t* - This will list the files sorted by modification date. Newest first
* **ls** *-r* - This will list the files in reversed fashion
* **ls** *-i* - This will list the *index node* number of each file in the current working directory

### the recursive option for ls
* **ls** *-R* - So if you want to list the contents of a directory and all it's subdirectories you use
* For example, Imagine if you have a directory named dir1 on your desktop, and inside dir1 you have a subdirectory named dir2. Now, if you type ls ­R dir1, Then this will list the contents of dir1 and dir2.
* Notice that if dir2 has another subdirectory dir3 then **ls ­R** dir1 will also list the files of dir3 and so on ... got it now ?
* Here comes the interesting part, if you executed **ls ­R /** then this will list all the files (non hidden) on your system

## Combining command options
* **ls** *-R* *-a* - list all the files including hidden files on your system | or **ls** *-Ra*
* You can also write it as **ls -a -R** or **ls -aR**, order doesn't matter
* **ls** *-Ra /* - will list all files on your system
* **ls** *­-latR /* - will make a long listing of all the files on your system sorted by modification date (newest first)
* Command options are case sensitive -R (Recursive) is not same as -r (reverse listing)

* If you want to list the files in reverse order based on time then we can combine *-­r* & *-­t* so , ls *-­tr* will list the files sorted by modification date (Oldest first)

## touch command
*(accepts multiple arguments)*

* **touch** *<file_name>* - modify timestamp of file
* **touch** *<file_name>* - make a new file if it does not exists

## mkdir command
*(accepts multiple arguments)*

* **mkdir** *<dir_name>* - make a new directory 
* **rmdir** *<dir_name>* - removes an empty directory

## rm commands
* **rm** *<file_name>* - remove a file (without any prompt)
* **rm -R** *<dir_name>* - remove a dir (empty or populated, without any prompt)
* **rm** *-Ri* *<dir_name>* - remove a dir, with a prompt
* **rm** *-i* *<file_name>* - will ask for confirmation before deletion, (*i* stands for interactive)
* **rm** *-f* *<file_name>* - delete a file, **forcefully** *this will ignore non-existent files, will not raise an error*
* **rm** *-v* - *v*, stands for verbose, it gives summary of your command
* **rm -R <file_name> <dir_name>** - to delete a file and a folder together

## cp commands
* **cp** *<source_file> <desired_file_name>* - copy file to same dir, can use paths to copy remotely located files
* **cp** *-R* *<source_dir> <desired_dir>* - copy dir 
* **cp** *-i* *args* - prompt you before any action like overwrite (i = interactive)
* **cp** *-v* - gives summary of actions done in the command ( v = verbose )

## Rename file
* **mv** *<old_filename> <new_filename>* - rename files
* **mv** *<old_filename> <.filename>* - make a file hidden (with same name)
* **mv** *<.filename> <filename>* - make a file unhidden
* **mv** *<file_1> <file_2> <destination_dir>* - move a file to a desired dir
* **mv** *<dir_1> <dir_2>* - move dir_1 to dir_2
* **mv** *-i <file> <destination>* - move/overwrites the file with a prompt

## file command
* **file** *<file_name1> <file_name2>* - print contents and file extension (file1 and file2 can be of another type)

## include space in filenames (3 ways)
* **mkdir** *'<dir_name>'* - make a dir including space in filename
* *can use double qoutes ("") also*
* *precede any space with a backslash*
* **mkdir** *file\ name* *file\ \ name*

**NOTE - same with rmdir**

## include special character in filenames
* **mkdir** *\$dollar* - include \ as a prefix
* **mkdir** *\&\<\'\;\\hello* - one "\" for one special char
* we can't include / in filename

*special chars in shell/terminal $ < > & | ; " \ '*

## some keyboard shortcut for terminal
* *Ctrl+a* - take you to start of command
* *Ctrl+d* - work as delete key, delete cursor keyword
* *Ctrl+e* - go to end of line
* *Ctrl+f* - move forward one key (same as right key)
* *Ctrl+b* - move backwards one key (same as left key)
* *Alt+f* - skip one word
* *Alt+b* - skip on word (backwords)
* *Alt+u/l* - transform a lowercase/uppercase word into uppercase/lowercase word
* *Ctrl+u/k* - cut the whole before/after cursor
* *Ctrl+y* - paste the line that you just cut
* *Ctrl+l* - clear screen

# file eidtors
* **gedit** *<file_name>* (GUI)
* **nano** *<file_name>* (CLI)
* **less** *<file_name>* - only for viewing file (CLI)

# cat and tac commands
* **cat** *<filename>* - print file contents to the terminal
* **cat** *<file1> <file2>* - show the file contents, combined
* **tac** *<file>* - view file contenst in reverse order

# head and tail commands
* **head** *<file_name>* - will only show u starting 10 lines of your file (default)
* **head** *-n 20 filename* - show starting 20 file lines

*vice and versa with **tail**.*

# wc command
* **wc** *<file_name>* - file file content info as *line number*, *word number*, *numbers of bytes/characters*
* **wc** *-l <file_name>* - show only line numbers
* **wc** *-w <file_name>* - show only words
* **wc** *-c <file_name>* - show number of bytes/characters
* **wc** *-L <file_name>* - print number of characters of the longest line

# There are 4 diff types of commands
* Executable Programs - found in bin folder like cp like a program
* Shell builtins - like built in bash like cd
* Shell scripts - files that contain code commonly found in bin or usr/bin
* Alias - define or create your own commands, is made with other commands e.g *ls*

* **type** *<command_name>* - tell nature of command, does not shows diff between exec command and shell script, for that
* *file* *path* like **file /bin/cp**

* *except shell builtin commands, all commands are executables*

*print out command path of executable commands* **which <command_name>**, but for shell builtin command will not print anything

**help <command_name>** - help guide for specific for shell builtin command, won't work for executables

**man <command_name>** - help guide for executable commands

**whatis <command_name>** - brief description about your command, won't work for shell builtins

# run multiple linux commands in single line
* **command_1, command_2...** *it will skip the wrong one and continue executing other commands*

**OR**

* **command_1 && command_2...** *in this it will ignore all after one faulty/typo/incorrect command* **short circuit evaluation**