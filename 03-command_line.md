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

* pwd - show current working directory path
* mkdir <dir> - creating a directory
* rmdir <dir> - deleting a directory
* touch <file> - creating a file using `touch` command
* rm <file> - deleting a file
* mv <file> <new_name> - renaming a file
* ls -a - listing hidden files
* mv <dir+file> <new_dir> - copying a file from one directory to another
* cd <dir> - change directory
* chmod <permission_code> <file> - change file permissions
* info <command> - documentation for command

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

| Command  | Action |
| ----     | ---- |
| ls       | lists contents of current directory
| ls -a    | lists contents of current directory, including hidden files |
| ls -l    | lists contents of current directory, plus content attributes | 
| ls -lh   | lists contents of current directory, plus content attributes and uses unit prefixes to reduce the length of file sizes |
| ls -lah  | lists contents of current directory, including hidden files, plus content attributes and uses unit suffixes to reduce the length of file sizes |
| ls -t    | lists contents of current directory, in order of last modified |
| ls -Glp  | lists contents of current directory, plus content attributes, colored and denoted by type |

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

* ls -a
* ls -r
* ls -R
* ls -t
* ls -1

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs is used to accept standard input as arguments for a command. It separates 'pieces' at whitespace and repeats the initial command. For example this describes the typical progression of cuisine when camping, taking and then echoing two foods at a time:

echo "apple banana potato onion marshmallow chocolate" | xargs -n 2

giving the output:
apple banana
potato onion
marshmallow chocolate

