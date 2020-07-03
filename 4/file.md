# run multiple linux commands in single line

* **command_1, command_2...** *it will skip the wrong one and continue executing other commands*

**OR**

* **command_1 && command_2...** *in this it will ignore all after one faulty/typo/incorrect command* **short circuit evaluation**

# wildcards
Wildcard is a symbol that represents one or more characters
e.g * this symbols matches any character, ? matches a single character

like for copying large number of files with diff names

? is useful when you have specific number in mind in the unknown area

we can combine them also

# create your own commands

* **select name that is not used in any command**
* **alias <command_name>="mkdir folder;date;cal"**
