# This is the most used commands of Git and Github. 
This page contains a number of Git and Github most used features 
The first section
`<br><br>`

# Git commands for local repository
## 1. Initialize git in a directory 
To initialize git in a directory run below command 

```
git init  
```



## 2. Configure Git 
To configure Git run below commands. 
```
git config –-global user.email "user-email" 
```
```
git config –-global user.name "user-name"  
```



### 3. Move changes in staging area 
To move a file or folder into stagin area, run below command

```
git add file-name.extension | ./directory-name
```

To move all files and folders into stagin area, run below command
```
git add .
```


## 4. Move changes out of staging area 
To move back a file & dir from staging area, run below command 
```
git rest file-name | directory
```
To move back all files & directories from staging area, run below command 
```
git rest .
```
OR 
```
git checkout -- file-name 
```


## 5. Commit the files & folders 
To commit file staged contents, run belwo command
```
git commit -m "write the commit message here"
```

### Add another change to your previous commit
When you miss to include a file in your commit or you make a mistake in your commit message, use this command 
```
git add the_change // to add the change 
```
and 
```
git commit -m "Update your commit message" --ammend 
```


### Log your Commits/Versions 
This will print all of your activity / active commits 
```
git log 
```
Output: 
```
commit 5b7708018570bbc4a6edeafe86766a7e9ac0d805  //commit id or hash id
Author: gitID <someone@somain.com>
Date:   Mon May 1 11:31:03 2023 +0800

    commit message
```

OR 
```
git reflog 
```
Output : 
```
da2045f HEAD@{1}: commit: app3 commit
b1f61c9 HEAD@{2}: commit: app2 commit
d22f193 HEAD@{3}: commit (initial): app1 commit
```

### Move to a specific Commit/Version 
```
git checkout commit_id
```


### Cancel a specfic Commit/Version
```
git revert commit_id 
```


## Get remote details 
Tip to get only the remote URL
```
git config --get remote.origin.url
```
OR 
```
git remote -v
```

In order to get more details about a particular remote, use the
```
git remote show [remote-name]
```
For example, below command show remote origin details.
```
git remote show origin
```

## Remove git from your directory completely 
```
rm -rf .git
```
