# Introduction to Git

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

### Commit

You will use a separate step to record (commit) those changes from the staging area to the source code control (your git repository) via the `git commit` command.  A committed change means that the data is safely stored in your local database.

![Git stage diagram](/static/assets/img/git-stage-diagram.png)

## What is GitHub?

[GitHub](https://github.com/) is a social, code hosting website.  If you are using Git on your laptop to provide version control for your project, GitHub will host for you for free (provided it is a public repo). GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.


[Home](/)  |  [Back to top](/intro/)  |  [Next](/intro/1)
