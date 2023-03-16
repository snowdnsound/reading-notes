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



