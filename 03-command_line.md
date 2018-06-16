# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command

* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 
* show current working directory path: pwd
* creating a directory: mkdir directory name
* deleting a directory: rm -r directory name
* creating a file using `touch` command: touch filename
* deleting a file: rm filename
* renaming a file: mv old filename new filename
* listing hidden files: ls -a
* copying a file from one directory to another: cp filename directory
* count how many lines a text file has: wc -l filename
* count how many words a text file has: wc -w filename
* look at the first 10 lines of a text file: head filename
* merge or concatenate content of files together: cat filename1 filename2





---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > 

`ls`: lists all files and directories in the working directory\
`ls -a`: lists all files and directories in the working directory, including hidden files\
`ls -l`: display the long listing of files and directories in the working directory\
`ls -lh`: display the long listing (including file sizes and date of mod)  of files and directories in the working directory in human readable format\
`ls -lah` display the long listing (including file sizes and date of mod) of files and directories in the working directory, including hidden ones, in human readable format\
`ls -t`: display  all files and directories in the working directory in order of time modified.
`ls -Glp`display the long listing of files and directories in the working directory while omitting group names and appending indicators to directories.

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 
ls -m: displays the names as a comma-separated list\
ls -r: displays files in revers order\
ls -R: displays subdirectories as well\
ls -u: displays files by the file access time\
ls -1: displays each entry on a line\

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs is used to build and execute commands from standard input. It converts input from standard input into arguments to a command.

For example, you can pipe the standard output of the echo command as standard input to another command:

# touch file.txt
is the same as
# echo file.txt | xargs touch

