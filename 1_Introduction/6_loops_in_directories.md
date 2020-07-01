# Create loops in directories

* **ln** *-s* *<abs_path>/<rel_path>/<..>* - create a loop using softlink

**Because hardlinks are not allowed for directories, loops can't be created with hardlinks**
