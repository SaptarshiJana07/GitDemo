# GitDemo
Author- Saptarshi Jana
# Tutoral
# Installing GitBash >> open it to configure
<br>  git config --global user.name "SaptarshiJana07"
<br>  git config --global user.email "mesaptarshi.jana@gmail.com"
<br>  git config --list

# see all files inside local repo $ initiate a git bash
All files: ```Get-ChildItem -Force```, Only Hidden: ```Get-ChildItem -Force -Hidden```
<br> show files: ```ls {any one of cmd}``` cmd: -Attributes, -Directory, -File, -Hidden, -ReadOnly,    
-System.
<br> Initiate git in the local repo: ```git init```
<br> clone the remote repo in local folder: ```git clone https://github.com/SaptarshiJana07/GitDemo.git```
# Workflow of Git in a Local Repo
Create a GitHub repo >> clone it with the local folder {PS G:\Git_local\GitDemo> ```git clone https://github.com/SaptarshiJana07/GitDemo.git```} >> make changes >> Add all changes {PS G:\Git_local\GitDemo> ```git add .```} >> Commit them with message {PS G:\Git_local\GitDemo> ```git commit -m "message"```} >> Push it to the GitHub {PS G:\Git_local\GitDemo> ```git push -u oginin main```} >> If you have made some changes at remote repo the sync it with local repo{PS G:\Git_local\GitDemo> ```git pull oginin main```}
<br> check the remote repo>> {```git remote -v```}

# to know the file status
>> PS G:\Git_local\GitDemo> ```git status```
== 1. Untracked 2. modified 3. Stagged 4. Unmodified
<br> Output: "On branch main
Your branch is up to date with 'origin/main'.
othing to commit, working tree clean"
<br> or 
On branch main---Nothing to commit
Changes not staged for commit: 
 modified:   README.md
  (Sol: use 1. "git add" and/or 2. "git commit -a")
  
  (Sol: use "git add <file>..." to stage (include/update) the changes, what will be committed)
  (Sol: use "git restore <file>..." to discard changes in working directory)
  
  (Sol: use "git commit -a <some_message>" to record changes in working directory)

# to stage the final change in the local repo (all together)

>> PS G:\Git_local\GitDemo> ```git add .```
check "git status"-- all stagged files will turn into green
# to save the final change in the local repo
>> PS G:\Git_local\GitDemo> ```git commit -m "new file added"```
# to push is to the Github cloud from local drive: remote repo is named as "origin" here.
>> PS G:\Git_local\GitDemo> ```git push origin main```
<br> >> PS G:\Git_local\GitDemo> ```git push origin branch1``` (in case of updating in the branch1 repo not the main)
# list your branches. a * will appear next to the currently active branch
<br>```git branch```
<br> create a new branch at the current commit
<br>```git branch [branch-name]```
<br> switch to another branch and check it out into your working directory
<br>```git checkout```
<br> merge the specified branch’s history into the current one
<br>```git merge [branch]```
<br> show all commits in the current branch’s history
<br>```git log```
<br>create branch: ```git branch -b person1```
<br>delete branch: ```git branch -d person1``` (after checking out from that branch)
<br>create branch: ```git branch -b person1```