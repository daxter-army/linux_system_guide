# Rename file

* **mv** *<old_filename> <new_filename>* - rename files
* **mv** *<old_filename> <.filename>* - make a file hidden (with same name)
* **mv** *<.filename> <filename>* - make a file unhidden
* **mv** *<file_1> <file_2> <destination_dir>* - move a file to a desired dir
* **mv** *<dir_1> <dir_2>* - move dir_1 to dir_2
* **mv** *-i <file> <destination>* - move/overwrites the file with a prompt

# file command
* **file** *<file_name1> <file_name2>* - print contents and file extension (file1 and file2 can be of another type)

# include space in filenames (3 ways)
* **mkdir** *'<dir name>'* - make a dir including space in filename
* *can use double qoutes*
* *precede any space with a backslash*
* **mkdir** *file\ name* *file\ \ name*

* *same with rmdir*

# include special character in filenames
* **mkdir** *\$dollar* - include \ as a prefix
* **mkdir** *\&\<\'\;\\hello* - one "\" for one special char
* we can't include / in filename

special chars in shell/terminal $ < > & | ; " ' \

# some keyboard shortcut for terminal
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