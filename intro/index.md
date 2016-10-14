# Introduction to Git

[Warmup](/intro/warmup)


## What is Git?

Git is an open source, distributed version control system designed for speed and efficiency.

> "By far, the most widely used modern version control system in the world today is Git. Git is a mature, actively maintained open source project originally developed in 2005 by Linus Torvalds, the famous creator of the Linux operating system kernel. A staggering number of software projects rely on Git for version control, including commercial projects as well as open source. Developers who have worked with Git are well represented in the pool of available software development talent and it works well on a wide range of operating systems and IDEs (Integrated Development Environments).  
Having a distributed architecture, Git is an example of a DVCS (hence Distributed Version Control System). Rather than have only one single place for the full version history of the software as is common in once-popular version control systems like CVS or Subversion (also known as SVN), in Git, every developer's working copy of the code is also a repository that can contain the full history of all changes." [What is Git](https://www.atlassian.com/git/tutorials/what-is-git)

## It's distributed

In a _centralized_ version control system, like Team Foundation Server (TFS) (Microsoft) or Subversion, you have a central server containing a central database.  Lose the central server, and you have some serious problems.


** Distributed Version Control system **

![distributed](/static/assets/img/distributed-vcs.png)


## How does Git manage my changes?

"Git thinks of its data more like a set of snapshots of a miniature filesystem. Every time you commit, or save the state of your project in Git, it basically takes a picture of what all your files look like at that moment and stores a reference to that snapshot. To be efficient, if files have not changed, Git doesn’t store the file again, just a link to the previous identical file it has already stored. Git thinks about its data more like a stream of snapshots." - [Pro Git](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

Many source control systems work at the file level.  Git is finer grained in that it tracks the _changes to a file rather than the entire file_.

### Staging Changes

Using the `git add` command tells git to that it should be interested in the  _changes made within in the file_.  Use `git add` to stage fixes to the staging area.  

### DEMO:  Create a NodeJS project and git repository from scratch

Using the command line interface (CLI), create a directory named hello-world, the beginnings of a package.json file, readme.md file, index.js file.

```
$ mkdir hello-world
$ cd hello-world
$ npm init -y
$ echo "# Hello World" >> readme.md
$ echo "console.log('Hello World!')" >> index.js
$ node index.js
```
### Exercise 2: Hello World

### DEMO: Create a repository, checking the status, and staging changes

Demonstrate the following commands wihtin our new NodeJS project:

```
$ git init
$ git status
$ git add
```

### Exercise 3: Create a repository, checking the status, and staging changes

### Commit

You will use a separate step to record (commit) those changes from the staging area to the source code control (your git repository) via the `git commit` command.  A committed change means that the data is safely stored in your local database.

![Git stage diagram](/static/assets/img/git-stage-diagram.png)

### Demo: Record changes to the repository

### Exercise 4: Record changes to the repository

### All the exercises...

Let's demo and then practice the remaining exercises.

[Home](/)  |  [Back to top](/intro/)  |  [Next](/intro/1)
