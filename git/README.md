### Repository

###### Clone Repo
> git clone url

###### Create Local Repo
> git init project_name

### Working with Branches

###### Create a new local branch
> git branch [branch-name]

###### Switch to another branch
> git checkout [branch-name]

###### Push a branch : From local to remote
> git push -u origin [Branch-name]

###### Delete a branch
> git branch -d [branch-name]

### Add/Undo File in Stage

###### Add a file to stage
> git add [file]

###### Remove file from stage (preserves contents)
> git reset [file]

### Committing Code

###### Committing file to the repository
> git commit -m Message

###### Committing file to the repository with Header and message
> git commit -m MessageHeader -m Message

### Undo Commits

###### Undo Commit - Preserve changes locally
> git reset [commit]

###### Undo Commit - Do not presever changes
> git reset --hard [commit]

### Reviewing History

###### List history
> git log

###### List history of a file
> git log --follow [file]

###### List of files changed for a commit
> git show --name-only 8ebb9e21a4525a3d311a6fef1b35b7529480aefd

###### Shows differences between two branches
> git diff [first-branch]...[second-branch]

###### Show difference of a file in two branches
> git diff branchname:file1 branchname:file2

###### See what has changed in a branch
> git whatchanged

###### See commit history of a file in gitk(ui)**
> gitk filename
