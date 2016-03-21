[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Git Basics

## Objectives

-   Initialize a git repository in order to track changes.
-   Create a new branch to isolate your changes.
-   Place new or changed files into the staging area to prepare them for a
commit.
-   Remove files from the staging area before a commit.
-   Commit new and changed files to a git repository.

## Prerequisites

-  [WDI Fundamentals, Chapter 2](http://fundamentals.generalassemb.ly/02_chapter/intro.html)

## Overview

-   Source control using only the file system
-   Why source control
-   What is a good commit message
-   Initialize repository
-   Initial commit
-   Branch, change, add, commit
-   Unstage changes

## Why Git?

Version control! As developers our code is our livelyhood so it's important
that we safely store our work... frequently.  Not only that we want to track our
changes as we make them.  If we make a feature that ends up breaking the rest of
our app we want to be able to go back to a point when our app was last working.

## Code Along: Making a Local Repository

Let's initalize a local repository.

1.In your training directory create a subdirectory called `game-of-gits`.

2.Inside of the `game-of-gits` directory create a file called `a-sad-tail.md`.

3.Opening the file with Atom copy in the following lines:

```bash
House Stark of Winterfell is led by the just Eddard "Ned" Stark, Lord of
Winterfell, Warden of the North, Hand of the King, Protector of the Realm,
Regent.  He is surely honorable and will lead a long and prosperous life.
```

4.Save the file.

5.Inside of the `game-of-gits` directory type `git status`. Did anything happen?

6.Again, inside the `game-of-gits` directory type `git init`.

7.Type `git status` again. Did anything happen this time?

## Demo: Linking with GitHub

So we have a local repository, watch as I create a GitHub repository.  Why
GitHub?  So we can backup our code online.  It also provides us with a useful
graphical interface and useful collaboration features.

Now create your own GitHub repository.

## Code Along: Staging and Commiting

Using `git add <"name_of_file">` we are going to add our story to the staging
area.

There are 3 states that your file can reside in `committed`, `modified` and
`staged`.  These states map to the different sections of a Git project.

```bash
Committed means that the data is safely stored in your local database. Modified
 means that you have changed the file but have not committed it to your database
 yet. Staged means that you have marked a modified file in its current version
to go into your next commit snapshot.
```
[Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

![Git Sections](https://git-scm.com/book/en/v2/book/01-introduction/images/areas.png)

When we add a file we are moving it from the working directory to the staging
area.

Now that our file is staged let's commit our file by typing `git commit`, Atom
should open.

## Lab: Crafting A Commit

Read over the following blog posts and carefully thing about what a good commit
message would be. Take some time to come up with your own. Be ready to share
your commit with the rest of the class.

-   [A Note About Git Commit Messages](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
-   [What's in a Good Commit?](http://dev.solita.fi/2013/07/04/whats-in-a-good-commit.html)

## Staging: And He Lived Happily After

Together, let's continue our story.

In our `a-sad-tail.md`, we'll tell the rest of Ned Stark's story.  Paste this in
below our current description and save:

```bash
Ned Stark went to King\'s landing and where he made lots of friends and lived
happily ever after...  He definitely did get axe murdered.
```

Now using what we learned earlier stage this change. To figure out the status
of your files you can type `git status` in the terminal at any time.

___Remember: Staging isn't commiting___

## Unstaging: Maybe We Jumpped the Gun

It turns out Ned actually did get axe murdered. So we probably want to unstage
our file.

Unstage the file with `git reset <"filename">`

Delete the last thing we wrote in `a-sad-tail.md`.

We know that Ned's story doesn't have a happy ending but let's dream big.  We're
going to create a dream-story branch and write what we would have wanted to
happen.

## Branching: Multiple Stories, One Main Plot

Similar to have one main story and various sub-plots a branch lets us
effectively duplicate and section off the code we have writte thus far, make
alterations to it, and if we would like at some point we can join it back to the
main branch (typically called `master`).

## References

-   [Git Commands Cheatsheet](command-reference.md)
-   [Learn Version Control with Git](http://www.git-tower.com/learn/git/ebook)
-   [Visualizing Git Commands](http://www.wei-wang.com/ExplainGitWithD3/)
-   [Learn Git Branching](http://pcottle.github.io/learnGitBranching/)

## [License](LICENSE)

Source code distributed under the MIT license. Text and other assets copyright
General Assembly, Inc., all rights reserved.
