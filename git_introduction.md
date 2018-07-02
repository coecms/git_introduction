# Git Introduction

## What is a version control system?

Tool developed for software development, but very useful also for anything text based. (i.e. LaTeX).
Solution to the mess you are almost certain to see:

    $ cd work/papers/precipitation_paper
    $ ls -1F
    old/
    bak/
    draft1/
    draft2/
    submitted/
    revised/
    submitted_v2/
    changes_from_sarah/
    changes_from_peter/
    final/
    final_v2/
    THIS_ONE/

So which one is the current version?
Does the `changes_from_peter` version also contain the changes from Sarah?
Or vice versa?

A version control system gets around all this chaos.
It keeps track of all changes, the order these changes were made, and why the changes were made.

### Advantages of git

Compared to older version control systems like subversion, git has two main advantages:

1. It's almost ridiculously easy to set up.
2. Its distributed infrastructure means that it does not need a central server.
   Though it can utilise one if desired.

## Initial configuration

Every commit you do will have your name and email address attached to it.

So, before you can use `git` the first time on your computer, you have to tell it who you are.

    git config --global user.name "Holger Wolff"
    git config --global user.email "Holger.Wolff@monash.edu"

This creates a file called `.gitconfig` in your home directory with these entries:

## Using git

### Creating a new repository

As I said before, creating a repository is ridiculously easy.
Just go into that directory, and type:

    $ git init .

And that's it.

We can now inquire about the repo:

    $ git status

As expected, it's empty.

### Pushing things into the repo



    git add
    git commit
    git commit -m
    git commit -a

## Getting things out of the repo

    git checkout
    git merge

## Cloud

## Useful aliases

    git config --global alias.ci commit
    git config --global alias.co checkout
    git config --global alias.st status
    git config --global alias.lg log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
