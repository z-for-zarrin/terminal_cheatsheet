# Terminal Cheatsheet
### A handy document to remember useful terminal commands
---

## Navigating Files
When you open your terminal, next to the green arrow is a prompt that will tell you which directory you are in. If you see a ``~``, you are in the home directory.

See the full file path of the directory you are in:
```pwd```
Should return something like /Users/zarrin-rahman

View a list of files and subdirectories in your current directory:
```ls```
- To view hidden files, add the flag ``-a`` to the end of the command.
- Similarly, add ``-l`` to view more details about the files.
- These flags can be chained together as follows.
```ls -al```

Change directory:
```cd Documents```
- Change "Documents" to any directory/path you wish to use.
- Use ``tab`` to autocomplete the names of files and directories.
- File names are case sensitive.

Go up a level in the directory path:
``cd ..``

Go back to the last directory you were in:
``cd -``

Return to home directory:
``cd``

## Creating & Manipulating Files
Create a new subdirectory in your current location:
```mkdir my_directory```

Create a new file in your current directory:
```touch my_file.txt```
- You can make different file types by changing the file extension, for example ``.png`` or ``.md``.

Rename a file:
```mv my_file.txt my_cool_file.txt```

Move a file:
```mv my_file.txt my_directory/my_file.txt```
- You can move and rename a file in the same command by writing the new name after the directory you wish to move it to.
- You can use ``mv my_file.txt ..`` to move a file up a level

Copy a file:
```cp my_file.txt my_directory```
- You can use ``cp my_file.txt ..`` to copy a file to the next level up

Copy a directory:
```cp -r my_directory our_directory```
- The ``-r`` flag stands for recursive

Delete a file:
```rm my_file.txt```

Delete a directory:
```rm -r my_directory```