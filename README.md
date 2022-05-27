#README.md file

.md -- Markdown file -- similar to markdown in Jupyter notebook.

Markdown has some shortcuts like a single #, which represents the main header.

#Git
'Git' is a version control system. It is free and open source. 

#Version control
Version control is the way through which the programmers track the changes in the code.
We basically save an initial version of our code into Git. When we update the code then we can save it into Git again. 
As we go on making the changes, if we want, we can look book at all the changes we have made to our code.
Basically, it helps us to understand what we did and when we did it.

#Terms
Repository -- It is the place where we put our code (or) save our code.
Git -- It is the tool that tracks the changes in our files over time i.e. it helps us in version control.
Github  -- It is the website where we host all of our Git repositories.

#Git commands -- all the commands are in lower case
clone -- Say, there is a repository that is not present on our local machine but it is on github and we want to bring it onto our local machine.
add -- when we have updated, created or deleted files and folders, we will want to tell Git that we have made changes and we want Git to track them. We use 'add'.
commit -- we know that Git is used to save the changes tha we have made in the code. Once, we 'commit', we are saving those changes in Git i.e. we are committing those changes.
push -- once we have made the changes locally on our computer and we are ready to put them on Git, we tell Git to track them through the 'add' command, we save our files to Git through the 'commit' command. 
And then we save (or) upload our files to a remote repository like 'Github' or 'Bitbucket'. We do this through 'push' command.
pull -- when there are changes to our code on Github and we want to download those to our local machine,we use 'pull' command i.e. we 'pull' down those changes from the repository.


#Create README.md -- it is the place holder text. If we do not write anything, it is taken as default.

#Say, we want to know see all the commits we have performed. We can see it in the --> code --> file --> upper right corner.
We can see that each commit has a unique identifier. 

#Green with '+' means that the line has been added to the file.
#Red with '-' means that the line has been deleted from the file.
#White means that it remained the same.

#In Mac and Linux machines, Git is inherently installed.

#ls -la -- in order to find out all the files and folders present in our repository.
#git status -- it shows all the files that have been updated, created or deleted, which have not been saved by commit yet.

#git add
untracked file -- it means that git does not about this file yet. So, we need to tell git that it should track this file before we save it to git.
For this, we use 'git add' command.

If we say 'git add .', it means that we are asking the git to track all the modified files as well as the newly created or updated or deleted files. So, they will all be staged with git.

Or we can just mention the individual file or folder that we want the git to track i.e. 'git add file-name'.

After staging, check the status again. We will see that these changes have to be committed and 'our branch is up to date with origin/main.

#git commit
Whenever we commit, we must add a message so that we will later be able to identify and know what we have done and why we have done it.
So, the code looks like 'git commit -m "my message" '. Here, '-m' represents message.
We can also add a description here i.e. description of what we have done. We do it by adding another '-m'.
 So, the command looks like 'git commit -m "my message" -m "some description" '.
 
#git init
Say, we want git to track the code in a particular folder. Then we just need to cd to that folder and then run 'git init'. This will track the code in that folder.

If we want to make an already existing folder into a repository, then 'git init folder-name'.
If we pass 'ls -la' commands into it, we will be able to see '.git' file in both of them.

#.git
It is a directory and it contains everything that is related to our repository.
If we want to stop tracking a directory, then we just need to remove this '.git' directory.
We can remove it using  'rm -rf' command.

#rm -rf
This command is used to remove a file/folder from the current directory.

#.gitignore
Say, we have some files that we do not want to be tracked. In such cases, we make use of '.gitignore' file.
'touch .gitignore' -- use this command first. This creates the .gitignore file.
.gitignore is just a text file and we put inside it the names of the files that we want to be ignored.
While we mention the names of the files to be ignored, we can use the wildcard characters.

#git add -A
If we want to add all the files that are currently untracked or that we made changes to the staging area, we use the command 'git add -A'.
If not, we can add them individually.

#git reset
If we want to remove the files from the staging area, we use 'git reset' command. Code looks like 'git reset file-name'.
If we want to remove all the files from the staging area, code looks like 'git reset'.

#git commit
If we want to save the changes made to the files, we use 'git commit' command.
We can add a message regarding the commit. Then the code looks like 'git commit -m "message"'.

#git log
Say, we want to check the details of all the commits made and who made them, we use 'git log'.

#git clone
Now, say, we want to clone a remote repository into a directory we want.
This remote repository can be on internet or on our local machine.
The code looks like 'git clone <url> <where-to-clone>'.
Here, if the code looks like 'git clone <url> .' , it means thatit has to be cloned to the current directory.
 
#git remote
Say, we want information about the remote repository. For this, we use 'git remote' command.
 'git remote -v' -- it gives us the origin (or) source location of the remote repository

 #git branch
 'git branch -a' -- it gives us all the branches present in our repository, not just locally, but remtely as well.
 
 


