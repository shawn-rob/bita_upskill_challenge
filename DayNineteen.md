# Inodes, Symlinks and Shortcuts #

In this module we are working on linking a file to a shortcut. Before we get to that, there is a new player in the filesystem game -- **inode**. Inode is the database information given to a file. 

Multiple files can have the same inode. Those files are hard links, which is a shortcut to a file. It's not a backup though, as you can make changes in the hard link that will show in the file. 

If you create a symbolic link and delete the original file, the link will no longer work. 

<!-- I have a whole hootnanny of photos to add here -->