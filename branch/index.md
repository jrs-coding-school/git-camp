# Branching

Branching means you diverge from the main line of development and continue to do work without messing with that main line.

Git encourages workflows that branch and merge often, even multiple times in a day. Understanding and mastering this feature gives you a powerful and unique tool and can entirely change the way that you develop.

The default branch name in Git is `master`. As you start making commits, you’re given a `master` branch that points to the last commit you made. Every time you commit, it moves forward automatically.

![master-branch-commit-history](/static/assets/img/master-branch-commit-history.png)

The “master” branch in Git is not a special branch. It is exactly like any other branch. The only reason nearly every repository has one is that the git init command creates it by default and most people don’t bother to change it.

## Demo:  Creating a branch

What happens if you create a new branch? Well, doing so creates a new pointer for you to move around. Creating a new branch called `feature-album-images`. You do this with the git branch command:

```
$ git branch feature-album-images
```

This create a new pointer.  `HEAD` let's you know what branch you are currently on.

![master-branch-commit-history](/static/assets/img/new-branch.png)

## Demo:  Where is HEAD pointing?

Run `git log` to view where the `HEAD` is pointing.

```
$ git log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short
```

## Demo: Switch to the new branch

The `git checkout` command allows you to switch to the new branch.  This moves the `HEAD` to the new branch.  

```
$ git checkout feature-album-images
```

Viewing the log reveals the `HEAD` is now pointing to our new branch, instead of master.

![master-branch-commit-history](/static/assets/img/switching-branches.png)



[Home](/)  |  [Back to top](/branch/)  |  [Next](/branch/1)
