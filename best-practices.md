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
Word | Definition
--- | ---
Repository | A Git repository (or repo) is a directory that stores all the files, folders, and content needed for your project, including the versions and commits of those files. Repositories can be shared and copied (see: fork).
Clone | A copy of a repository ("a clone", noun) or the action of copying a repository ("to clone", verb). When cloning a repository into another branch, the new branch becomes a remote-tracking branch that can talk upstream to its origin branch (via pushes, pulls, and fetches).
Branch | A version of the repository that diverges from the main working project. Branches can be a new version of a repository, experimental changes, or personal forks of a repository for users to alter and test changes.


## Workflow
* **Commit related changes** - A commit should be a wrapper for related changes. For example, fixing two different bugs should produce two separate commits. Small commits make it easier for other team members to understand the changes and roll them back if something went wrong.

* **Commit early** - Don't wait until you have a completed code before commiting. Commit as soon as you have something substantial, like a code preamble, a first function, or a data-loading section.

* **Commit often** - Committing often keeps your commits small and, again, helps you commit only related changes. Moreover, it allows you to share your code more frequently with others. That way it’s easier for everyone to integrate changes regularly and avoid having merge conflicts. Having few large commits and sharing them rarely, in contrast, makes it hard both to solve conflicts and to comprehend what happened.

* **Write good commit messages** - Everytime you commit change you will have the option to write a message that describes those changes. It is important to write a short message every time you commit. Just one line is usually enough information. E.g. this is a good commit message: "Changed " and this is a good commit message "changed some things".

* **Don't commit large files or files that cannot be version controlled** - Large files, such as ~Gb of data should not be stored in a GitHub repo as it makes interacting with the repo extremely slow. Small amounts of data are ok to be stored in the repo, but generally GitHub repos are best suited to code. Similarly, files that cannot be tracked by the version control software should not be included; this includes pictures, pdfs, and videos. You can choose not to commit certain files that are in your local directory by creating a *.gitignore* file. (This is a rule that can sometimes be broken, for example if you want to include a pdf that won't change in the future for display purposes - usch as the pdf in this repo).


## Naming conventions
Adopting consistent repository and file naming conventions early will help make our GitHub page easy to use - especially for future researchers who join our group.

### Repositories

