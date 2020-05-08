# Linux
These are my notes on basic working of linux and commands used in the terminal.

## Day 1

* pwd - present working directory.
* / - signifies root folder that is the master directory in linux
* cd - change directory (typing only cd gives home directory)
* cd ~ - also home directory
* ls - list command. Shows directory listing (typing only ls lists home directory)
* cd / -  to go to root directory
* clear - clears up terminal space for us
* ls ~ - lists home directory
* ls .. -  lists one previous directory
* ls ../.. - lists two previous directory
* cd .. - go to previous directory
* cd ../.. - go to 2 previous directories
* ls -l - list the files in long format 
> gives rights of the file, user, size of file, date and time of file creation.<br>
> drwxr - xr -x are rights of various users. <br>
> drwxr - directory read write execute rights - for the user of system/owner<br>
> xr - execute and read are rights of the group<br>
> x - others only have the rights to execute <br>

## ls command 

* ls -a - lists hidden files also
* ls -al - combination of ls -a and ls -l. Gives hidden directories in long format. ls -la also does the same.
* ls -S - sort directory according to size
* ls -lS - sort according to size and list in long format.
* ls - alS - sort,list in long format, hidden folders too
* ls Documents/* .html - gives files in the documents directory that have .html extension. * is wild card.
* ls -lS > out.txt - saves the entries of ls -lS to out.txt.
* ls -d * / - lists out only the directories.
* man ls - gives manual for ls command.

## cd command

* cd - as it is cd would end us in home directory
* cd / - sends us to root directory
* cd ~ - home directory
* cd .. - go to previous folder or one folder above.
* cd ../.. - go to previous two directories.
* How to go inside the folder that has space in it's name. Let us assume folder name is My Books
> 1. cd My\ Books
> 2. cd "My Books"
> 3. cd 'My Books'

## cat command - (short for 'concatenate')

first use of cat command is to display the content of the files in the terminal.

* cat - only cat echoes the input we give. Press Ctrl + D to exit cat command
* cat list1.txt - Displays the content of list1.txt in terminal
> list1 line 1<br>
> list1 line 2<br>
><br>
> list1 line 3<br>
* cat list1.txt list2.txt - Displays content of list1 followed by list2 in terminal
* cat -b list1.txt - add line numbers in front of non blank lines
> 1  list1 line 1
> 2  list1 line 2
><br>
> 3  list1 line 3
* cat -n list1.txt - add line numbers in front of all the lines
> 1  list1 line 1
> 2  list1 line 2
> 3
> 4  list1 line 3
* cat -s list1.txt - reduce multiple blank lines to one blank line
> list1 line 1
>
> list1 line 2
> 
> list1 line 3
* cat -E list1.txt - adds $ symbol at the end of each line to dignify the end of line
> list1 line 1$<br>
> list1 line 2$<br>
> $<br>
> list1 line 3$<br>

