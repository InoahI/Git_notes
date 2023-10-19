# Git Tutorial

This tutorial guides you through the basics of using Git.

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
8. [Best Practices](#best-practices)
9. [Conclusion](#conclusion)

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

```bash
git commit -m "your commit message"
```

```bash
git init
#start coding and add files here
#go to github and create an empty repo
git remote add origin https://github.com/your-username/your-repo-name.git
git add .
git commit -m "upload to github"
git push -u origin main
```


```bash
git clone
```
