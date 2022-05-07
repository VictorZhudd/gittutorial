# What is git and Why git?
Git is the most used version control system used in this world. A version control system records changes made to our code over time in a online database called **Repository**. In there, we can see who had made changes in the project. This is very useful when multiple people are working on the same project. From **Repository**, all team member would able to get latest version or any prior version they desired.


# Installing Git
1. Download from [Official Website](https://git-scm.com/downloads)

[website pic](https://github.com/VictorZhudd/gittutorial/blob/main/git%20install1.JPG)



### In this tutorial, I will use windows version as a example 

![windows download version](https://github.com/VictorZhudd/gittutorial/blob/main/windows%20download%20version.JPG)

Choose the version that are compatible to your computer, after download the installation application, click on it, and it suppose come out with this

![git install1](https://github.com/VictorZhudd/gittutorial/blob/main/git%20install1.JPG) 

Click **Install**

after installation

![git install3](https://github.com/VictorZhudd/gittutorial/blob/main/git%20install3.JPG)



Click on **finish**, now you have **Git** in your computer

# Configuring Git

### There are 2 things you have configure in git 

- Name

- Email



  ### There are 3 level of configuration

  - system-All users
  - global- All Repositories of current user
  - local-current Repositories 

  *In here, it is suggested to use global level.*

  ### set User name

  $ git config -- global user.name "Firstname  lastname"
  

  ### set User email

  $ git config -- global user.email "example@email.com"
  check if your code looks like this
  ![pictures](https://github.com/VictorZhudd/gittutorial/blob/main/git%20username%20and%20email.JPG)
  
  (credit to Programming with Mosh https://www.youtube.com/watch?v=8JJ101D3knE&t=555s)

  ### set User Git Folder
  	mkdir myproject (*name this anyway you want
  	
  	cd myproject
	
	
	*mkdir* makes a new directory.

	*cd* changes the current working directory.
  


  

# Git Basic 
First we should set up a A Git repository. A repository is the folder inside a project. This repository will tracks all changes made to files in your project. 


## 1. set up a repository

​	$ git init 

Initialized empty Git repository in /Users/user/myproject/.git/. /Users/user is your userfolder located in your system drive(usually in c drive).


Now you have create a repository, now try to commit something. 


### 2. commit to that repository

1. create a file called "pratice files"
2. In your git cmd windows type $ git add <pratice files> 
	this code will add your file into staging area.
3. Now, if you want to make some changes, you could upload the changed files by the same method
	 git add -A
Then you could include a message.	
     git commit -m "changes updated"


   

# Git Branches
	

## 	1.  What is Branches

If you are working on a project with a lot of people and you want to make a change to the collective project that you are working on. Branches command will let make specific changes to the file in the repository without affecting other people’s work.    

## 	2. To begin creating a branch, type in the following command with a name for the branch “mybranch.”

git branch NewBranches

## 	3. Now, let's switch to the branch we just created. By type in the following command
	
	git checkout mybranch
## 	4.  Now let's create a file named branchtutorial.txt. let's make an upload to the branch by uploading the file we just created
	touch branchtutorial.txt
##	5. Now we can edit the the txt file and make some changes
##	6. Once we have finished changing the file , we can add it by using the add all command.
	git add
##	7. Then we can commit the new file into the branch
	git commit -m “new txt files”
##	8. If we want to change the branch between the main and the mybranch branch, you just need to use following command.
	git checkout master. or git checkout mybranch





   

# Git Stash

## 1. what is git stash

git stash temporarily save (or stashes) changes you've made to your working copy so you can work on something else, and then come back and re-apply them later on.
The git stash command is useful when you are not ready to commit and need to switch branches or if we want to reverse back to where you started. You can stash your work by using stash commands. These command can make you save your work in the stash
 


## 2. How to stash your work

1. First , we must begin by branching a new branch and lets called it stashtutorial. We do thatt by type in following command
	git branch stashtutorial


2.Then we want to make sure we are working on the branch we just created.
git checkout stashtutorial

3. Now, let’s create a .py file for our purpose here and lets call it testfile.py
git stash save “newtestfile”

4. Now lets see our stash by type in
git stash list

5.Now if we are ready to use the new file we will use the pop command, which will take the most recent stash and apply the changes within. Since we have only made one stash, it will apply the changes of that stash.
git stash pop

6. If there were multiple stashes, the pop command would not work, try this if you want to see the first file you stash 
stash@{0}
git stash apply stash@{0}

7. if we want to remove a specific stash, we can use the drop command, with the stash’s id
	git stash drop stash@{0}


# Git rebased

In Git, there are two  ways to made changes from one branch into another: the *Merge* and the *Rebased*.  Rebasing is  used to maintain a linear project history. if the main branch is updated and you want to merge your branch to the main branch cleanly, rebasing is your best choice.

### Rebased command

git rebase <base>

## Simple Git Cheat Sheet 

Git command is simple, here is a [cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf) you can use



## Simple Git Exercises

You have finished This tutorial, Here are some question you can as your own. 

1.  What is your Git Version?

2. Try to set up a repository

3. Make commit to your repository

4. Create a new branch

   
