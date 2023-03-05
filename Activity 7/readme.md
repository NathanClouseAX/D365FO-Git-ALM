Activity 7 – Create and Configure a Build pipeline

use YAML template from https://github.com/microsoft/Dynamics365-Xpp-Samples-Tools/tree/master/CI-CD/Pipeline-Samples if you don't have a build pipeline already
create a build pipeline tied to your x++ repo if you don't have one
update values so it will run in your repo, perform a test run

#upload artifacts

download nuget packages from LCS
From the LCS home page, go to the shared asset library
click on NuGet packages
select a version and download the following:
application suite build reference
application build referencecompiler tools
platform build reference

in devops click on artifacts
click create feed
give the feed a name, make sure "members of your azure activty directory" is selected
click "connect to feed" and select nuget
Use the info provided to create your nuget.config file

Create an LCS PAT
Sign in to your Azure DevOps account and navigate to your user settings by clicking on your profile picture in the upper right corner and selecting "Security".

In the Security page, click on "Personal access tokens" under the "TOKENS" section.

Click on the "New Token" button to create a new personal access token.

In the "New Token" dialog box, provide a name for your token in the "Name" field.

Under "Organization", select the organization that you want to create the token for.

Under "Expiration", select how long you want the token to be valid for. You can choose from a set of pre-defined values or set a custom expiration date.

Under "Scopes", select the access level that you want the token to have. You can choose from a set of pre-defined scopes or create a custom scope.

Click on the "Create" button to create your personal access token.

Copy the token value and store it in a secure location, as you will not be able to view it again once you close the dialog box.


use nuGet to upload packages from a cloud dev VM after downloading from LCS
nuget.exe push -Source "(FeedName)" -ApiKey az <packagePath>

update packages.config with specific versions for each packagePath
look at packages.config in activity directory for example
.gitignore, azure-pipelines.yml, and nuget.config files are also avaialble in that directory for review

from a cloud dev box
