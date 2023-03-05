Activity 4:

Create work item

Create branch for work item
Navigate to the work item that you want to create a branch from.

Click on the "Create branch" button in the upper-right corner of the work item's page.

In the "Create a branch" dialog box, select the repository that you want to create the branch in.

Choose a name for your branch. By default, Azure DevOps will use the work item ID and title as the branch name.

Choose a base branch for your new branch. This will typically be the branch that you want to branch off from (e.g., the main branch).

Choose whether to include work items in your branch. If you select this option, Azure DevOps will automatically link any work items associated with the parent branch to the new branch.

Click on the "Create" button to create your new branch.

Sync to VS
Open Visual Studio and navigate to your Git repository.

Open the Team Explorer pane by clicking on the "Team Explorer" button in the toolbar.

In the Team Explorer pane, click on the "Sync" button to open the Synchronization view.

In the Synchronization view, you'll see a list of local and remote branches. To sync a remote branch, simply click on the "Fetch" button next to the remote branch you want to sync.

Once the fetch is complete, you'll see any new commits on the remote branch in the Synchronization view.

If you want to sync your local branch with the remote branch, click on the "Pull" button next to the remote branch.

If there are any conflicts between your local branch and the remote branch, Visual Studio will prompt you to resolve the conflicts before merging the changes.

Once you've resolved any conflicts, Visual Studio will automatically merge the changes from the remote branch into your local branch.

If you want to push your changes back to the remote branch, simply click on the "Push" button in the Synchronization view.

If there are any conflicts between your local branch and the remote branch, Visual Studio will prompt you to resolve the conflicts before pushing your changes.

Make and commit changes
create a new file in the repository
stage it using visual studio

Open Visual Studio and navigate to your Git repository.

Open the Solution Explorer pane by clicking on the "Solution Explorer" button in the toolbar.

Right-click on the new file that you want to stage and select "Add" from the context menu.

In the "Add to Source Control" dialog box, make sure the file you want to stage is selected.

Click on the "Add" button to add the file to the Git repository.

After the file has been added, it will appear in the "Changes" pane in the Team Explorer pane.

To stage the file for commit, click on the checkbox next to the file in the "Changes" pane. This will move the file from the "Unstaged Changes" section to the "Staged Changes" section.

Once you've staged all the files you want to commit, enter a commit message in the "Commit Message" field in the "Changes" pane.

Click on the "Commit" button to commit your changes to the Git repository.

Finally, click on the "Push" button in the Team Explorer pane to push your changes to the Azure DevOps Git repository.

next
Open Visual Studio and navigate to your Git repository.

Open the Solution Explorer pane by clicking on the "Solution Explorer" button in the toolbar.

Select the file(s) you want to commit by clicking on them in the Solution Explorer pane.

In the Team Explorer pane, click on the "Changes" button to open the Changes view.

In the Changes view, you'll see a list of all the files you've changed or added.

Enter a commit message in the "Commit Message" field at the top of the Changes view. This message should briefly describe the changes you're committing.

Review the changes you're about to commit in the "Changes" section of the Changes view.

If you're satisfied with the changes, click on the "Commit All" button to commit all the changes.

After you've committed your changes, they will be available in the "Commits" view of the Team Explorer pane.

Finally, click on the "Push" button in the Team Explorer pane to push your changes to the Azure DevOps Git repository.


Create pull request
Navigate to the branch that you want to create a pull request for.

Click on the "Create Pull Request" button in the upper-right corner of the branch page.

In the "Create a pull request" dialog box, choose the target branch that you want to merge your changes into.

Enter a title and description for your pull request. These should describe the changes you've made and why they're important.

Review the changes that will be included in your pull request in the "Changed files" section.

If there are any work items associated with your changes, you can link them to your pull request in the "Work items" section.

If you want to request specific reviewers for your pull request, you can add them in the "Reviewers" section.

Finally, click on the "Create" button to create your pull request.

After you've created your pull request, it will be available for review by the target branch's owner(s) and any requested reviewers. They can review your changes and provide comments, suggestions, or requests for changes.

Once your changes have been approved, you can merge your changes into the target branch by clicking on the "Complete" button in the pull request page. If there are any conflicts between your changes and the target branch, you'll need to resolve them before you can complete the pull request.


Approve pull request
Navigate to the pull request that you want to approve.

Review the changes that are included in the pull request by clicking on the "Files changed" tab.

If you have any suggestions or requests for changes, you can add comments to specific lines of code by clicking on the "+" icon next to the line.

If you're satisfied with the changes, you can approve the pull request by clicking on the "Approve" button in the upper-right corner of the pull request page.

In the "Approve Pull Request" dialog box, you can choose whether to approve the pull request with or without additional comments.

If you choose to add comments, you can enter them in the "Comments" field. These comments will be visible to the pull request's author and other reviewers.

You can also choose whether to require changes to be made before the pull request can be completed. If you choose this option, the pull request will remain open until the author makes the required changes.

Finally, click on the "Approve" button to approve the pull request.

As part of the approval process, you can also select other options such as:

"Reset approval" - this will remove your approval from the pull request.
"Wait for author" - this will pause the pull request until the author resumes work on it.
"Complete" - this will merge the changes from the pull request into the target branch.
"Reject" - this will reject the pull request and prevent the changes from being merged.
By following these steps, you can approve a pull request in Azure DevOps and choose the options that best fit your team's workflow.