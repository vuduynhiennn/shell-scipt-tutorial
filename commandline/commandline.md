- to check calendar, you need to type the **cal** commmand as follows
	- cal

- change passowrd : all unix system requirei passwords to hep ensure that yoru files and data remain your own and that the system itself is secure from hackers and crackers. Following are the steps to change your password
	- **step 1** : to start, type passowrd at the command prompt as shown below
	
	- **step 2** : enter your old password the on you;re currently using 

	- **step 3** : type your new password. Always keep your password complex enough so that nobody can guess it. But make suare, you remember it.

	- **step 4** : you must verify the password by tuping it again

- listing directories and files : all date in unix organized into files. All files are organized into directories. These directories are organized into a tree-like struture called the filesystem you can use the **ls** command to list out all the files or directories available in a directory. FOllowing is the example of using ls command with -l option 


- system shutdown : the most consistent way to shut down a unix system properly via the commmand line is to use one f the following commands

	- **halt** : bring the system down immediately
	- **init 0** : powers off the system using predefined scripts to sysnchronize and clean up the system prior to shutting donw
	- **init 6** : reboots the system by shitting it donw completely and then restarting it
	- **poweroff** : shuts down the system by powering off
	- **reboot** : reboots the system
	- **shutdonw** : shutdown the system 

# METACHARACTER

metacharacters have s special meaning in unix. for example * and ? are metacharacter. we use * to match 0 or more characters, a question mark (?) matches with a single character

for example" `ls ch*.doc`

here * works as meta chracter which matchs with any character if you want to display all the files ending with just .doc then you can use the flowwing command

`ls *.doc`

# HDIDEN FILES
	

an invisible file is one, the first chracter of which is the dot or the preod character (.) unix programs (inclung the shell) use most of these files to store configuraiton information

some commong examples of the hidden files include the fiesl

	.prfile - the bourne shell (sh) initalization script
	.kshrc the korn shell (ksh) initaliztion script
	.cshrc the c shell sch initnlztion script

to lis the invisale files, the specify the -a option to ls 

.single got (.) this represents the curren direcotry
..double got (..) this represents the parten directory 

#COUNTRING WORDS IN A FILE

you can use the wc command to get a count fo the total of lines, wors, and chracters  contained in a file, Folliwng is simple example to see the information about the file created above here is the detail of all the four columns 

`wc filename1 filename2 filename3`


#### you can go in your home directory anytime using the follwing command 

here ~ indicates the home directory. suppose you have to go in any other use's home directory use the folliwng command cd ~user_name

to go in the last directo you can use the follwing command cd

# absolute/ relative pathnames

/filename/filename : this is absolute directory
filename/filenam: this is relative directory

# listing directories

to list the files ina directory you can use the following systeax

`ls dirname`

# REMIVING DIRECTORIS 

directoris can be delteted using the rmadir command as follows

`rmdir dirname	

note: to remove a directory make sure it is empty which means there should not be any file or sub directory this directour
you can remove tilles 


#RENAMING DIRECTORS

the mv (move) command can also be used to rename a directory 
the syntax is as follows 

`mv olddir newdir`

you can renama a directory mydirc to yourdir as follows

`mv mydir yourdir`

the directores . and ...

# CHANGEING PERMISSIONS 

to change the file or the directory permissions you use the chmod change mode command 

1. + : adds the designated permission (s) to a file or directory

2. - : removes the designated permissin(s) from a file or directory

3. = : sets the designated permission(s)

here is an example using testfile. Running ls -1 on the testfile shows that the file;s permision are as follow


#USING chmod with absolute permisions 

the second way to modify permissions with the chmod command is to use a number to specify each set of permissions for the file 
each permission is assigned a value as the following table shows and the total of each set of permission provides a number for that set

1. 0 : no permission

2. 1 : execute permission

3. 2 : write permission

4. 4 : read permission

5. read and execute 