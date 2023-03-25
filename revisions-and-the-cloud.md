# Revisions and the Cloud

## Version Control

Version control is a system that allows you to revist different versions. It also allows you to revert back to a previous version, track modications and compare changes. Mistakes are easy to correct with a VCS! There are a couple different versions of VSC (version control systems). Local, centralized and distributed. 

* Local VCS - entails one database on your hard disk that stores chagnes to files.
* Centralized VCS - a single server storing all changes and file versions, which can be accessed by various clients. 
* Distrubuted VCS - uses mirrored repositories created by clients for various simultaneous workflows.

## What is Git?

Git is a DVCS that stores data into a system ith snapshots. Each time you commit a new version of your project, Git creates a snapshot and store a reference.

Every change applied to a file is tracked by Git and these files reside in three main stages:

* Commmited
Data is securely stored in a local database
* Modified
ile has been changed but not commited to the database
* Staged
Flagged a file's chagned version to be commited in the next snapshot

## ACP

git add filename  
This tells git to include these changes in the next snapshot

git add README.md  
or  
add files together by leaving a space in between

or  
add all files at once to stage for a snapshot with:  
git add .

Files have now changed from red to green, 
Now we will commit the files!

git commit -m
-m is a flag (that says we want to add a message)
Place your message inside double quotes “”

-m “Demonstrating ACP first time:


Reference Links:  
https://blog.udemy.com/git-tutorial-a-comprehensive-guide/ 
  

Answer These Questions: 
What is Version Control?

* Version control is a system that allows you to revist different versions and allows you to revert back to a previous version.

What is cloning in Git?

* Cloning allows you to copy your repository from another server to work on it with a local machine. 

What is the command to track and stage files?

* git add filename

What is the command to take a snapshot of your changed files?

* git commit and use the -m flag to write a message about why you made a change

What is the command to send your changed files to Github?

* git push
