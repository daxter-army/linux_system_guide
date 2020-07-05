# Wildcards

* Wildcard is a symbol that represents one or more characters e.g * this symbols matches any character, ? matches a single character
* Like for copying large number of files with diff names
* **?** is useful when you have specific number in mind in the unknown area
* we can combine *** & *?* also

# Alias : Create your own commands

* **select name that is not used in any command**
* **alias <command_name>="mkdir folder;date;cal"**

## delete alias commands

**unalias "command_name"**
**alias** - lists out all alias commands

* NOTE - But by defalut *alias* will only work for current desktop session, therefore to make it permanent , we need to write it in a file named *.bashrc* in our home directory