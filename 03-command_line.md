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

```
$pwd               " will print the working directory path   " 
$mkdir sample_dir  " will make directory name sample_dir "
$rm -r sample_dir  " will remove directory name sample_dir "
$touch file_name   " will create an empty file nameed file_name"
$rm file_name      " will delete the file file_name "
$ls -lah           " will list all files even hidden files"
$mv file_name old_file " will rename the file_name as old_file"
$cp old_file new_file "will make copy of old_file as new_file"
$grep -i 'python'  " will find the occurance of python in the given directory'
$find ./ -name '*.py'  "will find all file which ends with .py extension'
$ssh user.name@        " login to remote server"
$cd -                  " go back to previous working dir"

```

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

> > REPLACE THIS TEXT WITH YOUR RESPONSE

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > REPLACE THIS TEXT WITH YOUR RESPONSE

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > REPLACE THIS TEXT WITH YOUR RESPONSE

 

