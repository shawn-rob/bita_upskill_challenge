# Who Has Permission? #

## WhO OwNs WhAt? ##

There are three permisisons - read, write, and execute. There are three owners of each set of permissions - user, group, and others. 

To change the permissions of owners and groups, you use: chown and chgroup. 

There are two ways to change the permissions of the files and directories: 
**chmod {u or g or o} {- or +} {r or w or x}**

The other way involves numbers: 4 for read, 2 for write, and 1 for execute. If none of them are to be available then 0 is used. Add the numbers for each set user/group/other. For full permissions would look like **chmod 777 file.txt**