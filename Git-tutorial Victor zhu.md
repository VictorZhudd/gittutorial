# What is git and Why git?
Git is the most used version control system used in this world. A version control system records changes made to our code over time in a online database called **Repository**. In there, we can see who had made changes in the project. This is very useful when multiple people are working on the same project. From **Repository**, all team member would able to get latest version or any prior version they desired.


# Installing Git
1. Download from [Official Website](https://git-scm.com/downloads)

[website pic](C:\Users\zhuho\Desktop\website.png)

![](C:\Users\zhuho\Desktop\website.png)

### In this tutorial, I will use windows version as a example 

![windows download version](C:\Users\zhuho\Desktop\新建文件夹\windows download version.JPG)

Choose the version that are compatible to your computer, after download the installation application, click on it, and it suppose come out with this

![git install1](C:\Users\zhuho\Desktop\新建文件夹\git install1.JPG) 

Click **Install**

after installation

![git install3](C:\Users\zhuho\Desktop\新建文件夹\git install3.JPG)



Click on **finish**, now you have **Git** in your computer

# Configuring Git

### There are 2 things you have configure in git 

- Name

- Email

- 

  ### There are 3 level of configuration

  - system-All users
  - global- All Repositories of current user
  - local-current Repositories 

  *In here, it is suggest to use global level.*

  ### set User name

  $ git config -- global user.name "Firstname  lastname"

  ### set User email

  $ git config -- global user.email "example@email.com"

  

  

# Git Basic 

## 1. set up a repository

​	$ git init 

Initialized empty Git repository in <location in your computer>

### 2. commit to that repository

1. git  add first-commit.py

2. use $ git commit -m "first commit" to include a message

   

# Git Branches

## 	1.  What is Branches

1. A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process.

## 	2. How to create branches

​	git branch NewBranches

##  	3. delete new Branches

​	

1. ### delete local branches

   git branch -d NewBranches

2. ### Delete global branches

   git push origin --delete NewBranches

   

# Git Stash

## 1. what is git stash

git stash temporarily save (or stashes) changes you've made to your working copy so you can work on something else, and then come back and re-apply them later on.

## 2. How to stash your work

1. Save changes to branch A.
2. Run `git stash`.
3. Check out branch B.
4. Fix the bug in branch B.
5. Commit and (optionally) push to remote.
6. Check out branch A
7. Run `git stash pop` to get your stashed changes back.

# Git rebased

In Git, there are two  ways to made changes from one branch into another: the *Merge* and the *Rebased*.  Rebasing is  used to maintain a linear project history. if the main branch is updated and you want to merge your branch to the main branch cleanly, rebasing is your best choice.

### Rebased command

git rebase <base>

## Simple Git Cheat Sheet 

Git command is simple, here is a [cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf) you can use



## Simple Git Exercises

You have finished This tutorial, Here is a exercise you can do on your own. 

1.  What is your Git Version?

2. Try to set up a repository

3. Make commit to your repository

4. Create a new branch

   