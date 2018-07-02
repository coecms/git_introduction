# Git Introduction

## What is a version control system?

Tool developed for software development, but very useful also for anything text based. (i.e. LaTeX).
Solution to the mess you are almost certain to see:

    $ cd work/papers/precipitation_paper
    $ ls -F
    old/
    bak/
    draft1/
    draft2/
    submitted/
    revised/
    submitted_v2/
    changes_from_sarah/
    final/
    final_v2/
    THIS_ONE/



## Advantages of git

## Initial configuration

    git config --global user.name "Holger Wolff"
    git config --global user.email "Holger.Wolff@monash.edu"

## Creating a new repository

    git init

## Pushing things into the repo

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
