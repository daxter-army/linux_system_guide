# View Inode Numbers

* **ls** *-i* - show inode numbers of all files in current directory
* **ls** *-i /* - show inode numbers of all files in root directory
* **ls** *-l* - show additional info like file size (bytes), owner etc about files present in current dir

# Create Hard/Soft links

* **ln <file_name> <hardlink_name>** - create a hardlink of the desired file
* **ln** *-s* **<file_name/dir_name> <softlink_name>** - create softlinks of the desired file

**NOTE - Hardlinks are not allowed for directories, they were allowed earlier, but they have been disabled now, because it was producing ambiguity in the file system**