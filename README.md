# Learn Git and Github

[Learn Git and Github](https://youtube.com/playlist?list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF) Course by Osama Elzero ❤

---

## 01 - What Is Git And GitHub ? Part 1

### What Is Git and Github?

- GIT is Distributed Version Control System

- Git Is Free and Open Source

- Github Is Source for Project and Sources [ GitLab, BitBucket ]

- Github Simplify Using Git

- You Can Use Git Without Github

- Git Has GUI

### Why You Must Learn Git?

- Devs Contribute to The Same Project

- You Can Revert Changes

- You Can Collaborate to Fix Issues

- You Can Collaborate to Create New Features

- You Can Solve Conflicts

- You Can Organize Features

## 02 - What Is Git And GitHub ? Part 2

### Words You Will Hear

- Repository

- Branch

- Local Repo

- Remote Repo

- Commit (Snapshot or Checkpoint In Your Local Repo)

- Clone [ From Local Or Remote ]

- Push [ Upload Local Changes to Remote ]

- Pull [ You Pull Changes From Remote Repo To Your Local ]

- Pull Request [ Tell Other About Your Changes To Pull It From Local To Remote ]

### Important Notes

- Create Repository For Every Project.

- Create A New Branch For Every Feature or Enhancement.

- No Need To Connect To Remote Repo When Working.

- Anyone Can Push and Pull Depend On Permissions.

- Github Or Any Host is The Centralized Server and Team PCs is Th Working Copies

## 03 - Create GitHub Repository And Clone It

```bash
git clone "Your Repository URL"
```

## 04 - Add, Reset, Commit And Progress

###### Add Files

```bash
git add <File> <File>
git add *.extension
git add *
```

###### Show Satus

```bash
git status
```

###### Commit Changes

```bash
git commit -m "Commit Message Here"
```

## 05 - Push Local Changes To Remote Repository

###### Show Branches

```bash
git branch
git remote -v
```

###### Push Changes

```bash
git push origin main
```

###### Add Files

```bash
git add <File> <File>
```

###### Commit Changes

```bash
git commit -m "Commit Message Here"
```

## 06 - Pull Changes From Remote Repository

###### Pull Changes From Remote Repository

```bash
git pull origin
```

## 07 - Everything About Git Configurations

###### Show All Configurations

```bash
git help config
```

###### Show User Email

```bash
git config --global user.email
```

###### Change User Email

```bash
git config --global user.email "Your Github Email Here"
```

###### Edit Configuration

```bash
git config --global --edit
```

###### Create New File

```bash
touch "File Name Here"
```

## 08 - Generate And Test Github Public Key

###### Generate Key

```bash
ssh-keygen -t rsa -b 4096 -C "Your GitHub Email Here"
```

###### Get Key To Copy

```bash
cat ~/.ssh/id_rsa.pub
```

###### Same Command Example in Windows "Change Osama With Your Username"

```bash
cat C:\Users\osama\.ssh\id_rsa.pub
```
###### Test Key And Connection

```bash
ssh -T git@github.com
```

## 09 - Create Repository From Existing Project

###### Create New Directory
```bash
mkdir "Your Directory Name Here"
```

###### Initialize Empty Git Repository
```bash
git init
```

###### Create Empty File
```bash
touch "Your File Name Here"
```

###### Show Status
```bash
git status
```

###### Add Files
```bash
git add <File> <File>
```

###### Commit File
```bash
git commit -m "Your Commit Message Here"
```

###### Add Repository
```bash
git remote add origin "SSH Repository URL"
```

###### Example
```bash
git remote add origin "git@github.com:OsamaElzero/Course.git"
```

###### Push Data
```bash
git push -u origin master
```

## 10 - Pull Requests With Real Examples

No Code 

## 11 - Everything About Aliases

###### Make Alias For Command "status"
```bash
git config --global alias.st status
```

###### Show Alias Content
```bash
git config --global alias.st
```

###### Test "status" Command
```bash
git st
```

###### Make Alias For Command "branch"
```bash
git config --global alias.br branch
```

###### Show Alias Content
```bash
git config --global alias.br
```

###### Test "branch" Command
```bash
git br
```

###### Make Alias For Command "commit -m"
```bash
git config --global alias.cm "commit -m"
```

###### Show Alias Content
```bash
git config --global alias.cm
```

###### Test "branch" Command
```bash
git cm
```

###### Show All Edits
```bash
git config --global --edit
```

## 12 - Branching And Merging

###### Show Branches
```bash
git branch
```

###### Switch To Branch
```bash
git checkout "Branch Name"
```

###### Delete Branch
```bash
git branch -d "Branch Name"
```

###### Create Branch And Switch To It
```bash
git checkout -b "Branch Name"
```

###### Move / Rename Branch
```bash
git branch -m "New Branch Name"
```

###### Merge Branch With Current Branch
```bash
git merge "Branch Name You Need To Merge"
```

## 13 - Mastering Stash Part 1

###### Create Text File With "Hello World" String Inside It
```bash
echo "Hello World" > about_readme.txt
```

###### Save Work To Stash
```bash
git stash
```

###### List Items in Stash
```bash
git stash list
```

###### Get Work From Stash
```bash
git stash pop
```

## 14 - Mastering Stash Part 2

###### Save Work To Stash
```bash
git stash
```

###### List Items in Stash
```bash
git stash list
```

###### Get Work From Stash
```bash
git stash pop
```

###### Save Work To Stash With Description
```bash
git stash save "Description Here"
```

###### Get Specific Stash
```bash
git stash pop stash@{2}
```

###### Delete Stash
```bash
git stash drop stash@{1}
```

###### Show Lastest Added Stash Content
```bash
git stash show
```

###### Show Specific Stash Content
```bash
git stash show stash@{1}
```

###### Empty The Stash
```bash
git stash clear
```

## 15 - Restore And Clean

###### Restore Staged Files
```bash
git restore --staged "File Name Here"
```

###### Show Files That Will Be Cleaned
```bash
git clean -n
```

###### Remove Un Needed Files
```bash
git clean -f
```

## 16 - Resetting The Head

###### Show Log File
```bash
git log
```

###### Reset Head
```bash
git reset --hard "Commit Hash Here"
```

###### Push Edits From Local To Remote With Force Flag
```bash
git push origin main --force
```

## 17 - Ignoring Files And Directories

###### gitignore contents

```bash
*.log
!vip.log
node_packs/
text.txt
```

[Git Ignore Reference](https://git-scm.com/docs/gitignore)

## 18 - Tagging And Releasing Part 1

###### Show All Tags
```bash
git tag
```

###### Add New Lightweight Tag
```bash
git tag "Version Name Or Tag Name Here"
```

###### Add New Annotated Tag
```bash
git tag -a "Version Name Or Tag Name Here" -m "Description Or Message"
```

###### Push Tag To Remote
```bash
git push origin "Tag Name Here"
```

## 19 - Tagging And Releasing Part 2

###### List All Tags Starting With v1.
```bash
git tag -l "v1.*"
```

###### Delete Tag
```bash
git tag -d "Version Name Or Tag Name Here"
```

###### Delete Tag From Remote
```bash
git push origin --delete "Version Name Or Tag Name Here"
```

## 20 - The End And Advices


[Git Handbook](https://www.amazon.com/Git-Version-Control-Cookbook-Productivity/dp/1782168451)