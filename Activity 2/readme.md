Activity 2:
create a branch,


Use everything we just went through to create a DevOps project, create repo with initialization, map it, add a yaml build pipeline and .gitignore. commit changes, push

#Create Instance and Project
Create an instance: https://learn.microsoft.com/en-us/azure/devops/user-guide/sign-up-invite-teammates?view=azure-devops#sign-up-with-a-personal-microsoft-account

create a project: Once you create your first organization, you will be prompted to create a project. Be sure to select "private" and use Git.
otherwise to go the organization then click "new project" in the upper right
expand "advanced" and confirm source control is Git
Click create.

#Create Repo and Init
init repo: go to repos > File, check add readMe, add VisualStudio .gitignore, click initialize

#Map to Dev Box
Connect to Main: use VS to map locally (not dev machine), update .gitignore with details below.

update VS location for where to create projects (options > project and solutions > locations)

build pipeline

```
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
```

Next, add the yaml file from from repo

Next, commit changes

#create build pipeline
In DevOps, go to pipelines > pipelines
click create pipeline
click on Azure Repos Git
Select your repo ( if prompted )
select "existing azure pipeline yaml file" ( if prompted ) then select file
click create

#Add branch protections
go to project settings
then go to permissions then click on build administrators, click on members, click add, find "(project name) build service" then click save
First add repo build service to build admins (search on project name)

Also need to add repo build servie to feed permissions (search on project name) later
click on artifacts
select feed created previous
click on the gear in the upper right
click permissions 
click add users/group
select reader then add user "(project name) build service" then click save


go to project settings then repository under repos
go to the policies tab, click the plus sign in the bottom pane
make sure "Protect the default branch of each repository" is selected think click create

enable "require a miniumum number of reviewers"
require min 1 reviewers (use 2 or more in real life)
enable "Check for linked work items"
check for lineked work items

enable "limit merge types"
limit merge types

click the plus sign for build validation (after you have a pipeline)
add build validation 
select build piepline
make sure "required" for policy requirement is selected, click save
