pwd
Prints the current working directory. This helps you know where you are in the file system.

mkdir git-for-devops
Creates a new directory named git-for-devops. This is where you will set up your Git project.

cd git-for-devops/
Changes the directory to git-for-devops. You enter the newly created folder to work in it.

ls
Lists files in the current directory. Since it's a new directory, it should be empty.

pwd
Checks the current directory again to confirm you're inside git-for-devops.

clear
Clears the terminal screen to make the output more readable.

git init
Initializes a new Git repository in the git-for-devops folder, making it ready to track changes.

ls
Lists files again, and you'll see a hidden .git folder created by Git for tracking.

touch nibba.txt nibbi.txt
Creates two empty text files named nibba.txt and nibbi.txt.

ls
Lists files to confirm the two new files are created.

git status
Shows the status of the working directory. It will show that the two new files are untracked.

git add nibba.txt nibbi.txt
Stages the two files for committing. This tells Git to start tracking the files.

git status
Checks the status again. The two files should now be staged and ready to commit.

git rm --cached nibbi.txt
Unstages nibbi.txt without deleting it, meaning it will no longer be tracked by Git, but the file will still exist locally.

git status
Checks the status again. You should see that only nibba.txt is staged for committing.

git add .
Stages all changes in the current directory. This stages both tracked and untracked files.

git status
Checks the status again to ensure all necessary files are staged.

git commit -m "First Commit"
Commits the staged changes with a message "First Commit". This saves the current state of the project in Git's history.

git status
Checks the status again. After the commit, there should be no pending changes.

git config --global user.name "Imran"
Sets the global Git username to "Imran" for all future commits.

git config --global user.email "imran@yahoo.com"
Sets the global Git email to "imran@yahoo.com" for future commits.

git config --list
Lists all Git configuration settings, confirming that the username and email are correctly set.

clear
Clears the terminal screen.

ls
Lists files in the directory again, confirming that your files are still there.

git status
Shows the current status of your project. After the commit, there shouldn't be any uncommitted changes.

git checkout -b dev
Creates a new branch called dev and switches to it. This allows you to work on a new feature separately from the main branch.

git status
Checks the status to confirm you're on the new dev branch.

vim nibbu.txt
Opens vim to create or edit a file called nibbu.txt. After editing and saving, this file will be available in the working directory.

git add .
Stages all changes, including the newly created nibbu.txt.

git commit -m "added nibbu"
Commits the new file with a message "added nibbu".

git log
Shows the commit history. This will display the commits you've made, including "First Commit" and "added nibbu".

git checkout master
Switches back to the master branch to possibly merge or review changes.

git log
Shows the commit history on the master branch. It will only show "First Commit" since the dev branch has its own commits.

history
Shows a list of all commands you've run in the terminal session, including the Git commands you executed.
