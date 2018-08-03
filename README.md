Playing around with Git
======

## Basic creation/working commands

  * git init //add new .git folder and begin tracking changes
  * git config --global user.name "NAME GOES HERE" //to set name for user config
  * git config --global user.email "email@email.com"  //to set email
  * touch .gitignore //create your ignore file
  * git add .gitignore //add to index
  * git reset //reset contents of index
  * git commit -m "message" //to commit with a small message (for self-explaining changes)
  * git commit --amend //replace tip of current branch by creating new commit
  * git status //current state of working tree
  * git log //log of commits

  **Doug's procedure :**
  * git init
  * [make changes]
  * git add > commit
  * git remote add origin [url]
  * git push -u origin master //-u = set upstream
---
## Working w/ remote repo

  * git clone <url OR path to local directory> <where to clone>
    * ex: git clone https://www.github.com/fidgetylyons/gitPlay . //clone gitPlay from my repo to current directory
  * git remote -v //verbose option shows remote url after name
  * git branch -a //all option shows both remote-tracking branches and local branches
  * git remote add origin https://github.com/fidgetylyons //add remote repo

  **To Push :**
  * git pull origin master //check to pull changes from other devs since you pulled last
  * git push origin master //origin is name of remote repo, followed by desired branch
---
## Some Vocab

  * Origin - shorthand name for the remote repo that project was cloned from, it's used instead of original repo's URL, makes referencing easier
  * HEAD - current branch. Your working tree is normally derived from the state of the tree referred to by HEAD, it's a reference to one of the heads in your repository
  * head - A named reference to the commit at the tip of a branch
  * index - A collection of files with stat information, whose contents are stored as objects. The index is a stored version of your working tree.
  * pull - to fetch it and merge a branch
  * push - get the branch’s head ref from a remote repository, find out if it is an ancestor to the branch’s local head ref, and in that case, putting all objects, which are reachable from the local head ref, and which are missing from the remote repository, into the remote object database, and updating the remote head ref
  * stash entry - object used to temporarily store contents of a dirty working directory and the index for future reuse
  * upstream - generally refers to the original repo that you have forked
  * origin - default upstream repository, most projects have at least one upstream project they track, origin is used for that purpose
  * downstream - you're downstream when you copy (clone, checkout, etc) from a repository
  * upstream - when you've make changes, you usually want to send them back "upstream"
---
More to come soon, wish me luck!

![Image](buckleUp.jpeg "Me, pushing to master")
