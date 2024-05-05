# GitDemo
Author- Saptarshi Jana
# Tutoral
# to know the file status
>> PS G:\Git_local\GitDemo> git status
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
>> PS G:\Git_local\GitDemo> git add .
check "git status"-- all stagged files will turn into green
# to save the final change in the local repo
>> PS G:\Git_local\GitDemo> git commit -m "new file added"
# to push is to the Github cloud from local drive: remote repo is named as "origin" here.
>> PS G:\Git_local\GitDemo> git push origin main
