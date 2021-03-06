# .env-config
Configuration for many aspects of development (Gradle, Vim, Git)


To use this configuration clone this repository into your home directory with:
```
git clone https://github.com/chennemann/.env-config.git
```

- - - -

## .bash-config

The purpose of this configuration is to organize .bashrc scripts in multiple files to keep it organized.
If you use git bash to manage your repositories you will now have a long list of available shortcuts you can use to fasten up your workflow. See below for a reference for all available shortcuts:

### Aliases

Since git aliases always require the 'git' prefix I decided to use bash aliases to workaround this requirement.
With aliases defined in .bashrc you can ommit the prefix and speed up your workflow. (A little...)
Another "feature" build into those aliases is the tolerance for typos.

#### 'git clone [url]' - Clones the repository from the specified url
```
 - cl
 - clone
```

#### 'git status' - Checks the status of the working directory
```
 - ss
```

#### 'git fetch && git status' - Fetches changes from origin and compares them to the working directory
_This shortcut is very useful to compare the local repository with the latest changes in the remote repository_
```
 - s
 - stat
 - stats
 - statsu
 - status
```

### 'git fetch --all --prune && git branch --all' - Fetches all changes from origin and removes invalid tracking references. Then it shows the list of available branches.
```
 - f
 - fetch
```

#### 'git pull' - Fetches changes from origin and tries to merge them
```
 - p
 - pll
 - pull
```

#### 'git push' - Push local commits to origin
```
 - psh
 - push
```

#### 'git push -u origin [name]' - Push local commits to new branch
```
 - po
 - psho
 - pshorig
 - pusho
 - pushorig
 - pushorigin
```
#### 'git branch [name]' - List all available branches or creates a new local one with the given name
```
 - b
 - branch
 - lbranch
```

#### 'git branch -m ([old name]) [new name]' - Renames the specified (or the currently checked out) branch
```
 - rb
 - rename
 - renameb
 - renamebranch
 - rename_branch
```

#### 'git branch -d [name]' - Deletes a branch
```
 - db
 - deleteb
```

#### 'git checkout -b [name] && git push -u origin [name] && git status' - Creates a new branch, switches to it and creates the remote branch for it as well.
```
 - cb
 - createb
 - createbranch
```

#### 'git checkout [file|branch]' - Checkout a file or branch
```
 - co
 - checkout
```

### 'git checkout master' - Checkout the master branch (Convenience alias)
```
 - com
```

### 'git checkout develop' - Checkout the develop branch (Convenience alias)
```
 - cod
```

#### 'git add [file]' - Track specific file
```
 - a
 - add
```

#### 'git add .' - Track all untracked files
```
 - aa
 - aall
 - adda
 - addall
 - add_all
```

#### 'git commit' - Make a new commit
```
 - c
 - comit
 - commit
```

#### 'git commit -m' - Make a new commit and specify the commit-message inline
```
 - cm
```

#### 'git add . && git commit' Add all untracked files and make a new commit
```
 - ac
```

#### 'git add . && git commit -m' Add all untracked files and make a new commit and specify the commit-message inline
```
 - acm
```

### 'git add . && git commit -m [message] && git push' - Add all untracked files and make a new commit with a specified commit-message and push the made commit to the repository (Example: acp "feat: Test something")
```
 - acp
```

#### 'git log' - Displays the commit log
```
 - dl           //  Display Log
 - sl           //  Show Log
 - l      
 - log
```

#### 'git diff' - Displays the diff of the tracked files in the repository
```
 - df
 - diff
```

#### 'git merge [branch]' - Merges the specified branch into the current branch
```
 - m
 - merge
```

#### 'git rebase [branch]' - Rebase the current branch to the tip of the specified branch
```
 - r
 - rebase
```

#### 'git stash' - Stashes the current modifications
```
 - stash
 - stsh
```

#### 'git stash apply' - Applies the latest stashed modifications
```
 - apply
 - as
```

#### 'git stash && git pull && git stash apply' - Stashes the latest modifications, pulls modifications from remote repository, applies the made stash over it.
```
 - spa
```

#### 'git reset' - Resets the current git index
```
 - reset
```

#### 'git update-index --assume-unchanged [file]' - This command is useful if you don't want to add your changes to the repository yet
```
 - ig
 - ignore
```

#### 'git stash && git checkout [branch] && git pull' - This command stashes all current changes and checks out and pulls another given branch
```
 - scop
```

#### 'git fetch -p && for branch in $(git branch -vv | grep ': gone]' | awk '{print $1}'); do git branch -D $branch; done' - Remove all non-remote branches
_This command is useful for cleaning up a repository with lots of local branches that are no longer in use._

```
 - rmg
 - rmgone
 - removegone
 - remove-gone
```


#### './gradlew clean' - execute the clean task of the gradle wrapper in the current directory
```
 - clean

```

#### './gradlew build' - execute the build task of the gradle wrapper in the current directory
```
 - build

```

#### 'exit' - Closes the current Terminal
```
 - e
 - ex
 - exti
 - exit
 - eixt
 - eitx
```

#### 'source ~/.bashrc' - Refreshes the current Terminal
```
 - refresh
```

- - - -
