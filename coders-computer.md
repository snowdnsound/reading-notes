# The Command Line

The Command Line (CL) is another name for that black box called Termainal that you may have entered commands into or see runnign in the background. It's a text based interface to a system where you can put in commands and it prints out feedback. Don't think of it as leaving the GUI behind, but more like adding to it. You can have as many command line windows open as you want, running tasks **simultaneously.** Typically you might have three windows open. 

- One for doing work in
- One for viewing ancillary data
- One for viewing manual pages

## So What is it Exactly?

`1 user@bash: ls -l /home/ryan`  
`2 total 3`  
`3 drwxr-xr-x  2 ryan users 4096 Mar 23 13:34 bin`  
`4 drwxr-xr-x 18 ryan users 4096 Feb 17 09:12 Documents`  
`5 drwxr-xr-x  2 ryan users 4096 May 05 17:25 public_html`  
`6 user@bash:`  

**Line 1** presents us with a prompt, which after we enter a command (ls) which is often the first thing you type, sometimes followed by a (CLA) command line argument (-l /home/ryan). Note that these two things **must** be separated by spaces. This CLA is also referred to as an "option", which are typically used to modify a command. They are usually listed before other aguments and represented by a dash "-" thingie.

**Line 2 - 5** is what gets output as a result of entering a command. Not all commands show an output, but that doesn't mean nothing is happening, like displaying sensitive data such as your password. Unless of course there was an error, which it would probably tell you, "hey that was not right."

**Line 6** Shows us a prompt again. This will appear once the command is done running and the terminal/CL is ready to receive another command. If no prompt is displayed, then it is probably still running (you will learn how do deal with this later).

## Opening the Terminal

* If you are on a Mac, press command key+space bar and type in "Termainal", then hit enter. Boom!
* If on Linux, look in Applications > System or Applicaions > Utilities
* Else If Windows, and intend to remotely login, use an SSH client like [Putty](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html)

## The Shell (Bash)

Within a termainal, you have a shell. This is the part of the OS that defines how the terminal will behave and looks after running commands for you. There are many shells available but the most common one is called "bash" (Bourne again shell) **PUN ALERT** a pun on Stephen Bourne, author of the Bourne shell. 

If you would like to know which shell you are using you can type the command into terminal:  
`echo $HELL`  
`/bin/bash`    
`user@bash:`  

# Basic Navigation

## Where Am I?

To figuure out where we are we will use the command "pwd" (Print Working Directory). This will tell you what the current working directory is. It can be easy to loose your place in the termainal so this is helpful. We can use "ls" as a command to tell us what is there. You can add optional parts by using brackets such as `ls [options] [location]`.  

We can use this command in more powerful ways, explored below:  

`1 user@bash: ls`
`2 bin Documents public_html`  
`3 user@bash:`  
`4 user@bash: ls -l`  
`5 total 3`  
`6 drwxr-xr-x  2 ryan users 4096 Mar 23 13:34 bin`  
`7 drwxr-xr-x 18 ryan users 4096 Feb 17 09:12 Documents`  
`8 drwxr-xr-x  2 ryan users 4096 May 05 17:25 public_html`
`9 user@bash:`
`10 ls /etc`  
`11 user@bash: a2ps.cfg aliases alsa.d cups fonts my.conf systemd`  
`12 ...`  
`13 user@bash: ls -l /etc`  
`14 total 3`  
`15 user@bash: -rwxr-xr-x  2 root root 123 Mar 23 13:34 a2ps.cfg`  
`16 -rwxr-xr-x 18 root root 78 Feb 17 09:12 aliases`  
`17 drwxr-xr-x  2 ryan users 4096 May 05 17:25 alsa.d`  
`18 ...`  
`19 user@bash:`  

**Line 1** is the most basic way to use the command and listed the contents of our current directory.

**Line 4** This is ls with a single command line option ( -l ) which means we are going to do a long listing. A long listing has the following:  
* First character indicates whether it is a normal file ( - ) or directory ( d )
* Next 9 characters are permissions for the file or directory
* The next field is the number of blocks 
* The next field is the owner of the file or directory (ryan in this case)
* The next field is the group the file or directory belongs to (users in this case)
* Following this is the file size
* Next up is the file modification time
* Finally we have the actual name of the file or directory

**Line 10** Has been ran with a command line argument ( /etc ). This tells "ls" not to list our current directory but instead to list that directories contents.

**Line 13** This is ls ran with both a command line option and argument. It did a long listing of the directory /etc.

**Lines 12 and 18** just indicate that I have cut out some of the commands normal output for demonstration purposes. When you run the commands you will see a longer listing of files and directories.


## Absolute & Relative Paths

When we refer to a file or directory in the command line we are referring to a path. There are two types of paths, "absolute" and "relative". We can use either type of path and the system will be directed to the same location. At the top of the structure is the root directory, denoted by a single slash "/" and inside of those are subdirectories.  

Absolute paths - specify a location (file or directory) in relation to the root directory. They always begin with a forward slash.  
Relative paths - specify a location (file or directory) in relation to where you currently are in the system. They do not start with a slash.  

`4 user@bash: ls Documents`  
`5 file1.txt file2.txt file3.txt`  
`6 ...`  
`7 user@bash: ls /home/ryan/Documents`  
`8 file1.txt file2.txt file3.txt`  
`9 ...`  

**Line 4** We ran ls providing it with a relative path. Documents is a directory in our current location. This will return different results depending on where we are in the system. For example, if we were in Cam's documents and not Ryans.  

**Line 7** We ran ls with an absolute path and so this command will provide the same output no matter regardless of our current location. 

Here are some more building blocks to build your paths with:

* ~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
* . (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
* .. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.

You can use any of these to build your paths and the best approach is whichever is most convenient to you!

## Jump Around

No this is not referencing that House of Pain song... let's use the command cd [location] (change directory) to move around the system. Typically it is ran with a single command line argument, which is the location we would like to go to. The location is specified as a path which can be an absolute or relative path. You can even use some of the building blocks from above like so:

`cd ~/Documents`  
`cd ../../`  

You can also use a handy tool called **Tab Completion** which will autocomplete as you start to type a path! 

# More About Files

## Keep in Mind with Linux

Everything is awes-... a file!  
A directory is a file, your keyboard (ready only) and monitor (write only) are a file. Keep this in mind and it will help you understand what is happening under the hood. 

Linux is an extensionless system. A file extension is usually a 2-4 character set at the end of a file like Picture.png or Document.txt.  In other operating systems, like Windows, this is important and the system uses it to determine the file type. Linus is also case senstive, unlike Windows which is not. Another thing to keep in mind is when using spaces in names. A space on a command line is how we seperate CLAs. If we typed "Holiday Photos" the terminal would see these are two different arguments. We can solve this in two ways:  

Quotes - we can put single or double quotes around the item "holiday photos" 
Escape Characters - we can use a backslash which escapes or "nullifies" the special meaning of the next charcter. Holiday\ Photos

(In the previous section we learnt about something called Tab Completion. If you use that before encountering the space in the directory name then the terminal will automatically escape any spaces in the name for you.)

## Hidden Files & Directories

If the file name "begins" with a "." then it is hidden. To make a file or directory hidden, all you need to do is make it with it's name beginning with a "." or rename it to be so. You can also do the reverse of this to make a file/directory unhidden. The command "ls" will not list hidden files, however we can use the command line option "-a" so that it does show what is hidden. 


# Answer

1. What are four important features to look for in a text editor?  
* an auto-complete
* an error checker
* having a preview of your code
* can change the color scheme to fit your vision comfort level


2. What do the following commands do?
pwd - shows you where you are in the system
ls - lists the files in current directory 
cd - allows you to change directory
mkdir - makes a new folder/directory
touch - makes a new file

3. Can you explain what is happening in the following scenario if these commands and arguments are entered into the command line?
  
cd projects  
- this changes the directory to location projects

mkdir new-project
- This creates a new folder called "new-project"

touch new-project/newfile.md
- this make a new file with extension .md

cd ..
- this moves you back a directory and the number of dots equates to how far you go back

ls projects/new-project
- this would list the contents of what is inside the new-projects folder
















