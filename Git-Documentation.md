# Github Documentation

## Check Git Status
``` git status ```

## Clone a repository
Makes a clone of the online to your local

```git clone repository-link-here```

## New Issue

Before we begin any code, we must create a new Github issue. Ensure you assign it yourself and also label it with the correct tag (Bug, Enhancement, Feature, etc)

## New Branch
After you have created a new issue, we need to create a new branch in our local VS Code solution.

To create a new branch use the command:
>Must not have any spaces in the name.

``` git checkout -b branch-name-here ```

## Adding a new file

When adding a new file, you need to add it to the repository.

```git add (filename)```

## Commit locally
You commit locally first, then push to github later.

Go on the source control manager, enter a comment and press control + enter;

## Pushing
To push to github type 

```git push```

If there is no branch on the origin, you will be asked to create one.
>Always make sure this is the same name as your local branch.

```git push --set-upstream origin Useful-links```

You can continously type ``git push`` to keep updating the GitHub branch online. This is essentially the same as shelving the branch.

## Pull requests
After completing git push, you will need to login into GitHub online and create a pull request.

Ensure you assign the issue you created to the pull request. This is done by just typing #(ISSUE NUMBER) in the comment field. 

Here you will be able to see the changes etc.

## Merge Changes
Once a pull request has been completed, merge any changes by clicking Merge Changes.

## Switch branches
You may want to switch branches you are in/go back to master. 

To do this type:

``git checkout branch-name``

If you need to see a list of branches type 

``git branch``

## Updating your local solution with the master

After you have committed your branches and merged all changes, you need to update your local master. 

First switch back to the master branch

``git checkout master``

To then "pull" down the latest master source code, type

``git pull``

If you now type ``git status`` it should say your branch is up to date with 'origin/master'

## Deleting a branch

Once you have successfully merged and deleted the branch online, it is safe to delete from your local solution. To do this type

``git branch -d branch-name-here``

## To add an existing solution to a new github 

Create a github respository

``git init``

``git remote add origin link-to-dot-git-file``

Commit your changes

``git push -u origin master``

## Update branch from master

If your branch is outdated from the master. First checkout your branch 

``git checkout OutdatedBranch``

``git rebaes master``





