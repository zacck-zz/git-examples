# git-examples

Hello There

************ ADDING FILES
You can Use git add -A . to add all files to the re repo to the staging area

You can use git reset <filename> to remove files from the staging area.


************ ADDING FILES TO STAGING
staging area a place to put completed little taskss before combining them to your other work by "committing"

A commit is a snapshot of how your work looks at a certain point in time if we need to see chabes we made or someone else does


********** ADD NEW FILES TO REPO
Added a new file to the Repo as an example

*********USE GIT LOG
git -log --summary to see information about youe commits

********* ADD A REMOTE TO YOUR GIT
git doesnt care what your remote names are
but typically you name your main one origin  


********   HOOKS
You can use hooks to push your code to a server or a production build hosted somewhere. Whenever you push to your master instead of using an ftp or ssh client.


******* PULL
You may want to pull before having to commit some changes on option here  is to stash other than committing

git stash
to keep

git stash apply
to reapply uncommitted changes after pull


********** CHECK CHANGES
use git diff HEAD to check what changes we made during our last commit

The HEAD is a pointer that holds your position within all your different commits by default it points to the most recent commit without having to use the SHA

******* USING GIT DIFF

use -- staged to check what files have been changed and staged

****** UNSTAGING

oh oh you messed up you can unstage files using git reset command


*********** UNDO
So you were fractally wrong and you want to go back before this whole mess
files can be changed back using
git checkout -- target
          ^^^^ not the space betweeen the pointers and file name

*********** USING BRANCHES
Branches are what naturally happens when you want to work on multiple features at the same time. You wouldn't want to end up with a master branch which has Feature A half done and Feature B half done.

you can use branches to segment your work and only commit once that section is done

use git checkout -b branch_name to create and move to a new branch

When Branching and You want to add a new branch on the server repo remember to use
git push --set-upstream origin example_branch


************* REMOVING THINGS

Use git rm '*.*' to remove all the things in your repo

or git rm -r folder
to remove a specific directory  or you can use a filename to remove just on file


Remember when you remove things you should also commit your changes

also you can use the -a flag to make sure deleted files are auto removed

********PULL REQUESTS
If you're hosting your repo on GitHub, you can do something called a pull request.
A pull request allows the boss of the project to look through your changes and make comments before deciding to merge in the change. It's a really great feature that is used all the time for remote workers and open-source projects.
Check out the pull request help page for more information.



********** MERGING BRANCHES

use git merge example_branch

 to merge example_branch to master

Merge Conflicts
Merge Conflicts can occur when changes are made to a file at the same time. A lot of people get really scared when a conflict happens, but fear not! They aren't that scary, you just need to decide which code to keep.
Merge conflicts are beyond the scope of this course, but if you're interested in reading more, take a look the section of the Pro Git book on how conflicts are presented.
