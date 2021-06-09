# Git/Github best practices for our team
*Written by Matt Allcock, 04/06/21*


## Introduction
This document provides a best practice guide for using Git and GitHub for version control of code within our team.


## Definitions
Git has a bunch of terminology that is specific to version control workflows. Here are some of the most common terminology.

### General

Word | Definition
--- | ---
Version control | The practice of tracking and managing changes to software code. 
Git | The most popular version control software. Using a specialised command line, users can track changes made to code and other text files in a way that minimises space requirements and makes the used of cumbersome file version names redundant.
GitHub | A popular provider of internet hosting for software development and version control using Git.

### Git-specific
Approximately in order of importance/usefulness.

Word | Definition
--- | ---
Repository | A Git repository (or repo) is a directory that stores all the files, folders, and content needed for your project, including the versions and commits of those files. Repositories can be shared and copied (see: fork).
Commit | The "commit" command is used to save your changes to the local repository.
Remote | A remote is a common repository that all team members use to exchange their changes. For us, a remote repository is any repository stored on our GitHub server. This contrasts with "local", which is the diretory on your computer that your Git is working in.
Push | Updates a remote branch with the commits made to the current branch. You are literally “pushing” your changes from local onto the remote.
Clone | A copy of a repository ("a clone", noun) or the action of copying a repository ("to clone", verb). When cloning a repository into another branch, the new branch becomes a remote-tracking branch that can talk upstream to its origin branch (via pushes, pulls, and fetches).
Branch | A version of the repository that diverges from the main working project. Branches can be a new version of a repository, experimental changes, or personal forks of a repository for users to alter and test changes.
Merge | Taking the changes from one branch and adding them into another (traditionally master) branch. These commits are usually first requested via pull request before being merged by a project maintainer.
Fork | Creates a copy of a repository.
Pull/Pull Request | If someone has changed code on a separate branch of a project and wants it to be reviewed to add to the master branch, they can put in a pull request. Pull requests ask the repo maintainers to review the commits made, and then, if acceptable, merge the changes. For our GitHub, we will all be repo managers so will all be able to merge our own pull requests. A pull happens when adding the changes to the master branch.
Master | The primary branch of all repositories. You can work directly from the master branch, or create other branches.
HEAD | HEAD is a reference variable used to denote the most current commit of the repository in which you are working. When you add a new commit, HEAD will then become that new commit.


## Workflow
* **Commit related changes** - A commit should be a wrapper for related changes. For example, fixing two different bugs should produce two separate commits. Small commits make it easier for other team members to understand the changes and roll them back if something went wrong.

* **Commit early** - Don't wait until you have a completed code before commiting. Commit as soon as you have something substantial, like a code preamble, a first function, or a data-loading section.

* **Commit often** - Committing often keeps your commits small and, again, helps you commit only related changes. Moreover, it allows you to share your code more frequently with others. That way it’s easier for everyone to integrate changes regularly and avoid having merge conflicts. Having few large commits and sharing them rarely, in contrast, makes it hard both to solve conflicts and to comprehend what happened.

* **Write good commit messages** - Everytime you commit change you will have the option to write a message that describes those changes. It is important to write a short message every time you commit. Just one line is usually enough information. The message should be descriptive and concise. E.g. this is a good commit message: "Finished the function that calculates return levels" and this is a good commit message "changed some things".

* **Don't commit large files or files that cannot be version controlled** - Large files, such as ~Gb of data should not be stored in a GitHub repo as it makes interacting with the repo extremely slow. Small amounts of data are ok to be stored in the repo, but generally GitHub repos are best suited to code. Similarly, files that cannot be tracked by the version control software should not be included; this includes pictures, pdfs, and videos. You can choose not to commit certain files that are in your local directory by creating a *.gitignore* file. (This is a rule that can sometimes be broken, for example if you want to include a pdf that won't change in the future for display purposes - usch as the pdf in this repo).

* **Write a README file for every repository** - A README file is a text file that gives an overview of the repository. What you include in the README depends on the type of repository. Some examples of what could be included in a README: description of files, instructions of how to download/install software.


## Naming conventions
Adopting consistent repository and file naming conventions early will help make our GitHub page easy to use - especially for future researchers who join our group.

### Repositories

