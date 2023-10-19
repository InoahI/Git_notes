# Git Notes

This guide introduces the basics of using Git, offering a corresponding command cheatsheet. If you're unfamiliar with any commands, consult the official documentation by executing the command below:
```bash
git help <command>
```

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Basic Git Concepts](#basic-git-concepts)
4. [Git Commands](#git-commands)
    - [Initializing a Repository](#initializing-a-repository)
    - [Tracking Changes](#tracking-changes)
    - [Branching and Merging](#branching-and-merging)
    - [Remote Repositories](#remote-repositories)
    - [Undoing Changes](#undoing-changes)
5. [Collaboration](#collaboration)
    - [Cloning a Repository](#cloning-a-repository)
    - [Pushing and Pulling](#pushing-and-pulling)
    - [Pull Requests](#pull-requests)
6. [Advanced Topics](#advanced-topics)
    - [Rebasing](#rebasing)
    - [Git Hooks](#git-hooks)
8. [Wonderful Resources](#wonderful-resources)


## Introduction

Git is a powerful version control system that helps you manage your codebase, track changes, and collaborate with other developers. Whether you're working on a personal project or contributing to open-source software, Git is an essential tool for modern software development.

## Getting Started

### Installing Git

Before you begin, you need to install Git on your computer. You can download Git from [https://git-scm.com/](https://git-scm.com/) and follow the installation instructions for your operating system.

### Configuration

After installing Git, you should configure your username and email address. Open a terminal and run the following commands, replacing `<Your Name>` and `<your@email.com>` with your actual information:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

## Basic Git Concepts

### Repositories: 
 A Git repository is a directory that contains all the files and history for a project.
### Commits: 
Commits are snapshots of your project at a specific point in time. Each commit has a unique identifier and contains changes made to the files in the repository. So that you can always go back when you make mistakes.
### Branches: 
Branches are independent lines of development in Git. You can create a new branch to work on a feature or bug fix without affecting the main codebase.
### Merging: 
Merging is the process of combining changes from one branch into another.

## Git Commands

### Initializing a Repository
Before you can start tracking projects with Git, you need to initialize a repository. This creates a new .git subdirectory in your project folder.

```bash
git init
```




### Tracking Changes
Once you've made changes in your project, you can stage those changes to prepare them for a commit.
```bash
git add <file-name>
```
Or stage all changes:
```bash
git add .
```
Commit staged changes:
```bash
git commit -m "message of the description of the changes"
```
### Branching and Merging
Create a new branch:

```bash
Create a new branch:
```

Switch to an existing branch:

```bash
git checkout <branch-name>
```
Merge changes from another branch into your current branch:
```bash
git merge <branch-name>
```
### Remote Repositories
After creating a repository on platforms like GitHub, you can link your local repository to the remote one:
```bash
git init
#start coding and add files here
#go to github and create an empty repo
git remote add origin https://github.com/your-username/your-repo-name.git
git add .
git commit -m "upload to github"
git push -u origin main
```
If you successfully executed the code above( don't forget to change the path in URL), you should see the remote repo after running the code below
```bash
git remote -v
```


### Undoing Changes
To discard changes in a file:
```bash
git checkout -- <file-name>

```
To unstage changes:
```bash
git reset <file-name>
```


To undo a commit:

```bash
git revert <commit-id>

```

## Collaboration
### Cloning a Repository

To get a copy of a remote repository on your local machine:

```bash
git clone <repository-url>


```

### Pushing and Pulling

Push changes to a remote branch:

```bash
git push origin <branch-name>

```
Pull changes from a remote branch:

```bash
git pull origin <branch-name>


```

### Pull Requests

Pull requests are a feature of platforms like GitHub and GitLab. They allow developers to suggest changes that can be merged into the main codebase. To create a pull request, push your branch to the remote repository and use the platform's UI to open a new pull request.


## Advanced Topics 

### Rebasing

Rebasing is a method of integrating changes. It works by moving the entire commit history of a branch to a new base commit:

```bash
git rebase <branch-name>


```

### Git Hooks

Git hooks are scripts that can be run automatically before or after certain Git commands. They are stored in the .git/hooks directory of a Git repository.

## Wonderful Resources
[Git Documentation](https://git-scm.com/doc)\
[Pro Git](https://git-scm.com/book/en/v2)\
[GitHub Learning Lab](https://lab.github.com/)\
[Git Immersion](https://gitimmersion.com/)\
[Atlassian's Git Tutorials](https://www.atlassian.com/git/tutorials)\
[Git Explorer](https://gitexplorer.com/)\
[Interactive Git Visualization Tool](http://git-school.github.io/visualizing-git/)\
[Oh Shit, Git!?!](https://ohshitgit.com/)\
[Git for Ages - A git tutorial meant for all ages](https://github.com/acrylcandy/git-for-ages)
