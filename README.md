# This is the most used commands of Git and Github. 
This page contains a number of Git and Github most used features 
The first section
`<br><br>`
## Git commands for local repository
### 1. Initialize git in a directory 
To initialize git in a directory run below command 

```
git init  
```




### 2. Configure Git 
To configure Git run below commands. 
```
git config –-global user.email "user-email" 
```
```
git config –-global user.name "user-name"  
```



### 3. Move file in staging area 
To move a file or folder into stagin area, run below command

```
git add file-name.extension | ./directory-name
```

To move all files and folders into stagin area, run below command
```
git add .
```


### 4. Reset staging area
To move back a file & dir from staging area, run below command 
```
git rest file-name | directory
```
To move back all files & directories from staging area, run below command 
```
git rest .
```


### 5. Commit the files & folders 
To commit file staged contents, run belwo command
```
git commit -m "write the commit message here"
```



### Get remote details 
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
