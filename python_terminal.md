# Vij Prework - The Command Line


1. **[The Command Line](https://ryanstutorials.net/linuxtutorial/commandline.php)**
* bash is short for Bourne again shell  
* the up and down arrows are awesome short cuts to repeat commands  

2. **[Basic Navigation](https://ryanstutorials.net/linuxtutorial/navigation.php)**
* pwd is Print Working Directory  
* ls is the command line followed by [options][locations]  
* ls -l will list out all the files with more information  
* \- indicates file and d indicates directory  
* then we have the file size and finally who it belongs to and also name of the file or directory  
* ls -l /etc will list out the contents of the directory  the config files
* when writing absolute paths, you can use the ~ for the root directory  
* \. refers to the current directory  
* \.. refers to the parent directory  
* ls ~ (refers to contents of /users/vijayeter)
* ls / (lists contents at / level before users)  

3. **[More About Files](https://ryanstutorials.net/linuxtutorial/aboutfiles.php)**  
* when you have file or directory names with a space in them, and then you later try to open them, the terminal will see the space and word following it as an argument rather than part of the name.  So for it to work - either type \ before the space, or use tab to auto complete it and it will fill using \ or enter the whole word in quotes.   
    >*  for example: cd 'Holiday Photos' or cd Holiday\ Photos
* case sensitive
* >everything is a file  
* in linux, there are no extensions  
* >\. are hidden files

4. **[Manual Pages](https://ryanstutorials.net/linuxtutorial/manual.php)**  
* to see manual pages for a command type
  >* for example: man ls
  >* type q to quit manual pages  
* you can type man -k [search term] to find terms in the manual pages especially when you cannot remember the command  
* ls -alh lists all files including hidden files and the sizes are expressed in KB

5. **[File Manipulation](https://ryanstutorials.net/linuxtutorial/filemanipulation.php)**  
* >touch to create file
* >mkdir create a directory
* >mkdir -pv ~/blah/blahblah/blahblahblah
  * here we made parent directories using -p command and -v to explain what is happening and then we can also determine location based on the absolute or relative path we choose  
* >cp\<source>\<destination> and cp -r for recursive for copying directories  
* >move files or directories using mv\<source>\<destination>  
* >rename directories using the move option  
* we can also run commands when we are not in the location where the change is happening  
* >rmdir is to remove directories and rm to remove files and rm -r to remove directories with all the contents.  

6. **[Vi Text Editor](https://ryanstutorials.net/linuxtutorial/vi.php)**  
* There are two modes in Vi. **Insert (or Input)** mode and **Edit** mode. In input mode you may input or enter content into the file. In edit mode you can move around the file, perform actions such as deleting, copying, search and replace, saving etc.  
  >* ZZ (Note: capitals) - Save and exit    
  >* :q! - discard all changes, since the last save, and exit  
  >* :w - save file but don't exit  
  >* :wq - again, save and exit  
* **View** files using cat (concatenate) command.
* >\<Ctrl> + c which is the universal signal for Cancel in Linux.  
* >less\<file>  
 For larger files there is a better suited command which is less.  
* **Other commands**
  >Arrow keys - move the cursor around  
j, k, h, l - move the cursor down, up, left and right (similar to the arrow keys)  
^ (caret) - move cursor to beginning of current line  
$ - move cursor to end of the current line
nG - move to the nth line (eg 5G moves to 5th line)  
G - move to the last line  
w - move to the beginning of the next word  
nw - move forward n word (eg 2w moves two words forwards)  
b - move to the beginning of the previous word  
nb - move back n word  
{ - move backward one paragraph  
} - move forward one paragraph  
u - undo last action
U - Undo all changes to the current line  

7. **[Wildcards](https://ryanstutorials.net/linuxtutorial/wildcards.php)**  
* Wildcards are a set of building blocks that allow you to create a pattern defining a set of files or directories.   
* It is actually bash that does the translation which means we can use them on the command line whenever we want.  
  > \* - represents zero or more characters  
  ? - represents a single character  
  [] - represents a range of characters  

* **Examples**  
  >[sv]* => file beginning s or v and any number of letters  
  >\*[0-9]* => file with number in range 0-9 within the name  
  >[^a-k]* => use the ^ to show that the letter should not include in the range a-k  
  >[[:upper:]] => for upper case letter  

8. **[Permissions](https://ryanstutorials.net/linuxtutorial/permissions.php)**  
* Permissions specify what a particular person may or may not do with respect to a file or directory. 
  >r read - you may view the contents of the file.  
w write - you may change the contents of the file.  
x execute - you may execute or run the file if it is a program or script.  

* For every file we define 3 sets of people for whom we may specify permissions.

  >owner - a single person who owns the file.   
  >group - every file belongs to a single group.   
  >others - everyone else who is not in the group or the owner.  

* For example:
  > -rwxr----x: - is file; rwx is permission for the owner; r-- for the group;  --x for others which is execute function only  

* chmod It stands for change file mode bits  
  > **chmod \[permissions] \[path]**  

  >\[ugoa] - user (or owner), group, others, all  
  >Granting or revoking the permission - indicated with either a plus ( + ) or minus ( - )  
  >read ( r ), write ( w ) or execute ( x )  

  **Examples**  
  > * chmod g+wx frog.png => changes two settings
  > * chmod go-x frog.png => changes on two modes  
  > * chmod 240 frog.png => using binary shorthand for user(2), group (4), others(0)  

9. **[Filters](https://ryanstutorials.net/linuxtutorial/filters.php)**  

1. Grep and Regular Expressions
1. Piping and Redirection
1. Process Management
1. Scripting
1. Cheat Sheet

