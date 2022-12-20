# important-git-code and instructions 
git code, I use often but never remember 

## MacOS
#### Don't Forget
- git reset --hard HEAD~1 (removes the last commit)
- rm -rf .git (removes tracking, but you may have to delete the git folder)
- CMD + shift + . (to see hidden files on MacOS like the git folder)
- touch .gitignore (creating gitIgnore file in repo)]
- git rm --cached FILENAME (to remove a particular file that has been added to the remote repo, filename should be file path)

#### Adding Stuff to gitignore
- just drag the file into the .gitignore txt window, remove /Users/Ibukunoluwa blah blah 
- for individual files just use the file name
- then add, commit and push :)

> 🚨 For android add / at the beginning of the file path

Examples
<br>

```
/app/release/
/app/build/outputs/
```

#### Cloning a repository and pushing back to the repo 
- git clone (the git url)
- and just start working like nothing happpened

#### Changing the Github User
- git config --global credential.username "new_username"

## Collaborative Stuff 🤝

### Branches
- git branch - To know what branch you're own 
- git branch 'branchName' - creates a new branch 
- git checkout 'branchName' - to move to a branch 

### Pulling
- git pull - to pull changes from the remote repository into working directory

### Stashing Commits and Pulling
If you want to pull changes into your working directory, you would have to commit the changes you've made so they are not lost. 
```
git add .
git commit -m 'commit message'
git pull
```

### Pulling From Master Branch into Your own Branch Like Master
This is important so you don't modify the code in master or destroy the branch
```
git checkout master
git pull

git checkout <your branch>
git merge master
```

### Puliing from Another branch into yours 
```
git pull
git merge origin timi
```

### Undoing a Commit that has not been pushed 
[Resource for Commit Deletion](https://www.junosnotes.com/git/how-to-unstage-files-on-git/#:~:text=To%20unstage%20commits%20on%20Git,and%20specify%20the%20commit%20hash.&text=Alternatively%2C%20if%20you%20want%20to%20unstage%20your%20last%20commit%2C%20you,order%20to%20revert%20it%20easily.&text=Using%20the%20%E2%80%9C%E2%80%93soft%E2%80%9D%20argument,your%20working%20directory%20and%20index.)
this removes the commit but your changes remain
```
git reset --soft HEAD~1
```

### Git Stash
[Resource for Stash](https://git-scm.com/docs/git-stash)

Git stash stores your current changes in a cache and resets the working directory to the last commit that was pushed so it appears like there are no new changes
The changes can now be reapplied with 

```
git stash apply
```

### Removing a large file from Github in a Commit that has not been pushed 
[Resource for Large File Deletion](https://medium.com/analytics-vidhya/tutorial-removing-large-files-from-git-78dbf4cf83a)
```
git rm --cached csv_building_damage_assessment.csv
git commit --amend -C HEAD
```


## Backend references
- [Tutorial: Create a web API with ASP.NET Core](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-7.0&tabs=visual-studio)
- [Dockerize your SQL Server and use it in ASP.NET Core with Entity Framework Core](https://www.twilio.com/blog/containerize-your-sql-server-with-docker-and-aspnet-core-with-ef-core)
- [How to containerize your ASP.NET Core application and SQL Server with Docker](https://www.twilio.com/blog/containerize-your-aspdotnet-core-application-and-sql-server-with-docker)

## Windows
#### Deploying ASP.NET Web Api
- Build > Publish > Folder Profile
- Create a Folder as your target
- Opening Server 
  - Windows + R to open run 
  - type mstsc
  - Type in the server address and whatever then login 
  
#### Redeploying 
- Open the bin file on the server
- Replace dll and pdb files that carry the solution name with the new one that was published 
