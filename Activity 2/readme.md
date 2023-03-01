Activity 2:

Use everything we just went through to create a DevOps project, create repo with initialization, create a branch, map it locally, add a yaml build pipeline and .gitignore. commit changes, push

Create an instance: https://learn.microsoft.com/en-us/azure/devops/user-guide/sign-up-invite-teammates?view=azure-devops#sign-up-with-a-personal-microsoft-account

create a project: Once you create your first organization, you will be prompted to create a project. Be sure to select "private" and use Git.

init repo: go to repos > File, check add readMe, add VisualStudio .gitignore, click initialize

Connect to Main: use VS to map locally (not dev machine), update .gitignore, add build pipeline

# Ignore everything
*

# You can be specific with these rules
#!/some/other/deep/path/**
!.gitignore
!/VSProjects

#include package, exclude binaries
!/AAXTest
/AAXTest/bin
/AAXTest/XppMetadata

!AXModulesBuild.proj
BuildProjectResult.err.xml
BuildProjectResult.log
BuildProjectResult.xml

Add branch protections:

Create new branch