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


### Cloning a bloody repository and pushing back to the repo 
- git clone (the git url)
- and just start working like nothing happpened

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
