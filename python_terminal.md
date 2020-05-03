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
    *  for example: cd 'Holiday Photos' or cd Holiday\ Photos
* case sensitive
* everything is a file  
* in linux, there are no extensions  
* \. are hidden files

4. **[Manual Pages](https://ryanstutorials.net/linuxtutorial/manual.php)**  
* to see manual pages for a command type
  * for example: man ls
  * type q to quit manual pages  
* you can type man -k [search term] to find terms in the manual pages especially when you cannot remember the command  
* ls -alh lists all files including hidden files and the sizes are expressed in KB

5. **[File Manipulation](https://ryanstutorials.net/linuxtutorial/filemanipulation.php)**  
* touch to create file
* mkdir create a directory
* mkdir -pv ~/blah/blahblah/blahblahblah
  * here we made parent directories using -p command and -v to explain what is happening and then we can also determine location based on the absolute or relative path we choose  
* cp\<source>\<destination> and cp -r for recursive for copying directories  
* move files or directories using mv\<source>\<destination>  
* rename directories using the move option  
* we can also run commands when we are not in the location where the change is happening  
* rmdir is to remove directories and rm to remove files and rm -r to remove directories with all the contents.  

6. **[Vi Text Editor](https://ryanstutorials.net/linuxtutorial/vi.php)**  

1. Wildcards
1. Permissions
1. Filters
1. Grep and Regular Expressions
1. Piping and Redirection
1. Process Management
1. Scripting
1. Cheat Sheet

To submit your work, copy the above list and paste each of your meaningful observations and learnings below each section as a way to illustrate and highlight things like 'ah hah' moments or really interesting code snippets.
    - _Please note: If you submit one-liners (i.e. "The permissions section talked about permissions. It was cool.")_ you will not receive credit for this assignment.
