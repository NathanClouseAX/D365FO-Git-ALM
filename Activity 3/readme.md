# Activity 3:

Use Git Command Line to perform a push, pull, fetch, and sync. Also confirm what branch you are currently working in via command line. Find the same info in Visual Studio.

Command Line

## getting started
Open the command prompt in Windows. You can do this by pressing the Windows key + R, then typing "cmd" and pressing Enter.

#cloning a repo
if you have already cloned a repo, you can skip this step
Navigate to the directory where you want to clone the Git repository. You can use the cd command to navigate to the directory. For example, if you want to clone the repository in the Documents folder, type cd Documents and press Enter.

Clone the Git repository from Azure DevOps using the git clone command. Type git clone <repository-url> and press Enter. Replace <repository-url> with the URL of your Azure DevOps repository.

## check status
Navigate to the cloned repository directory using the cd command. Type cd <repository-name> and press Enter. Replace <repository-name> with the name of your cloned repository.

Check the status of the repository using the git status command. Type git status and press Enter. You should see that the repository is up to date with the remote repository on Azure DevOps.

## basic commands
Make changes to a file in the repository. For example, you can add some text to the README.md file using a text editor.

Check the status of the repository again using the git status command. Type git status and press Enter. You should see that there are changes to be committed.

Add the changes to the staging area using the git add command. Type git add README.md and press Enter.

Commit the changes to the repository using the git commit command. Type git commit -m "Update README.md" and press Enter.

Push the changes to Azure DevOps using the git push command. Type git push and press Enter. You may need to provide your Azure DevOps credentials to authenticate.

Check the status of the repository again using the git status command. Type git status and press Enter. You should see that the repository is up to date with the remote repository on Azure DevOps.

Create a new branch using the git branch command. Type git branch new-branch and press Enter.

Switch to the new branch using the git checkout command. Type git checkout new-branch and press Enter.

Make changes to a file in the new branch. For example, you can add some more text to the README.md file using a text editor.

Add and commit the changes in the new branch using the git add and git commit commands.

Push the changes to Azure DevOps using the git push command. Type git push -u origin new-branch and press Enter. This will create the new branch on Azure DevOps and push your changes to it.

Switch back to the main branch using the git checkout command. Type git checkout main and press Enter.

Merge the changes from the new branch into the main branch using the git merge command. Type git merge new-branch and press Enter.

Push the changes to Azure DevOps using the git push command. Type git push



## Using VS

commit - https://learn.microsoft.com/en-us/visualstudio/version-control/git-make-commit?view=vs-2022

add - https://learn.microsoft.com/en-us/visualstudio/version-control/git-line-staging?view=vs-2022

push - https://learn.microsoft.com/en-us/visualstudio/version-control/git-push-remote?view=vs-2022

fetch, pull, sync - https://learn.microsoft.com/en-us/visualstudio/version-control/git-fetch-pull-sync?view=vs-2022
