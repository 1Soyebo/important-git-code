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
