This is an exercise for the information that I will put in to this repo. 
The markdown file is used also as notes from basics in git


Key features in git:

1) Open the Terminal and find the folder that contains the Git project
2) Open VS or another code editor available that allows us to edit code efficiently and quickly
3) Run in Terminal "git status" to make sure nothing is needed to be changed
4) Once complete, save files to the folder (normal save)
5) To make changes available for branching, do "git add (either branch name or "." for all)" in the terminal to stage the changes
6) Check again under "git status" that this is what you wanted
7) Once confirmed, run "git commit -m 'MESSAGE'" to commit the changes
8) If you want to push this to the repo online (github.com), run "git push (repo web link) BRANCHNAME" for specific branch or "git push (repo web link)" for all branches



Several notes on common practices:

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
If there is a long message, usually resolving error in the terminal, you have to do Shift + Colon (write colon) and type "wq" to exit the message!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

When adding a new feature or new change, utilize a new branch in the process. To do this, follow these steps:
    1) Run "git checkout -b BRANCHNAME(NEW)". This is the shortned meathod that combines two parts
        a) "git branch BRANCHNAME(NEW)"
        b) "git checkout BRANCHNAME"
    2) Do neccessary changes and follow above as written

If you're in the process of merging this branch data to the primary branch/main branch, follow these steps
    1) Make sure you are on the branch (usually main) that you would want to merge into using "git checkout BRANCHNAME(host)"
    2) Run "git merge BRANCHNAME(target)" The new branch that is listed here will merge into the hosted branch listed from the step above
If there is an error, resolve accordingly. If edits were made on the main branch while the offshoot branch was worked on, then you can decide to keep code either in VS or delete the error codes or lines of code that you didn't want.

To checkout out the history of log and accessing them, use this:
    1) Run "git log --oneline". The "--oneline" makes it easier to see the versions that we would need to see
    2) Copy the version you are looking to see
    3) Run "git checkout VERSIONID" to see the changes. It will adjust the files but you wont change the actual files. This is where you can either branch out or do other things from the version selected

    To go back to the most current version, checkout to the most recent version:
    4) Run "git checkout main" or whichever the name it was assigned to

To add a file in the branch, either use VS or do this in the Terminal
    "touch filename.filetype"