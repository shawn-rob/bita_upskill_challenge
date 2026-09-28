# More or less is the name of this game. #


I am a bit far behind but better late than never right. 

This day is about more or less. Getting a feel on linux commands.
Less/more is for viewing files and getting to the top and/or bottom.

### Determine File Size ###

I learned two commands well two commands from a command: ls -a and ls -l. One shows all the files and directories including the hidden ones(ls -a) and the other shows the permissions, size, ownership, and modification time(ls -l). While there are so many combinations for ls. Those two are the main ones I have used during this challenge.

### * EDIT * ###

ls -lhS(That's an uppercase S) puts the filesizes in easier reading format. I can see the files in order and with the bits as M or K respectfully. 

The three largest files are **auth.log** at 4.8M, **btmp** at 4.3M, and **syslog** at 1.4M.

### How Many Lines ###

**wc -l** is the command in order to see how many lines occupy a file. wc on its on means word count. The large file **auth.log** contains *40936* lines and 473921 words and 4.9M characters, while a smaller log **fontconfig.log** only has 16 lines and 73 words and 789 characters.

Using **head** and **tail** shows you the first or last ten lines. Using -n and the number you can specify just how many lines you want to display.

**grep** will locate a word within a file. grep -i is used to perform a case-insensitive search.