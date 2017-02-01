+++
title = "Git Overview"
date = "2017-01-22T18:05:18-05:00"
toc = true
next = "/00-dev-tools-github/github-tutorial"
prev = "/00-dev-tools-github/tools"
weight = 4

+++

## What is Git?

- Version control for Programmers

- Like Microsoft Word "Track Changes" feature with superpowers

- Makes it easy for programmers to collaborate and work on the same codebase

- SVN (subversion) and CVS are other version control programs (Git is the most popular)


----

## What is Github?

- Web-based Git repository hosting service

- Built on top of git

- Home to +90% of all **open source** projects

- Morphed into a "social network" for developers


----

## Vocabulary

- Repository
- Commit
- Branch
- Merge
- Push
- Pull
- Fork
- Clone
- Pull Request

----

## Respository

- Most basic element of GitHub

- A repository contains all of the project files

- Stores each file's revision history

- Repositories can have multiple collaborators and can be either public or private.

----

## Commit

- A "revision", is an individual change to a file (or set of files)

- Git's version of "saving"

- Commits usually contain a commit message which is a brief description of what changes were made


----

## Branch

- Parallel version of a repository

- It is contained within the repository, but does not affect the primary or master branch allowing you to work freely without disrupting the "live" version.

- When you've made the changes you want to make, you can merge your branch back into the master branch to publish your changes

----

## Merge

- Merging takes the changes from one branch (in the same repository or from a fork), and applies them into another

- This often happens as a Pull Request (which can be thought of as a request to merge)

----

## Push

- Refers to sending your committed changes to a remote repository such as GitHub.com

- For instance, if you change something locally, you'd want to then push those changes so that others may access them

----

## Pull

- Pulls code from a remote repository and merges it with code in your local repository (on your computer)


----

## Fork

- A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project

- Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea


----

## Clone

- Copies a remote repository down to your computer and creates a link between the two


----

## Pull Request

- Pull requests are proposed changes to a repository submitted by a user and accepted or rejected by a repository's collaborators. 
- Pull requests each have their own discussion forum. See Using Pull Requests.
- Used to perform "Code Reviews" of other developers' work



{{% notice tip %}}
  Great resource for all things git can be found [here](https://git-scm.com/book/en/v2)
{{% /notice %}}

