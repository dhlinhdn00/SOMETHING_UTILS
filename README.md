# Basic Git Guide for Beginners

## Introduction

Git is a distributed version control system that helps developers manage changes to source code and projects over time. This guide will cover the basic Git commands and concepts needed to get started.

## Installing Git

Before using Git, you need to install it on your computer:

- **Windows**: Download the installer from [git-scm.com](https://git-scm.com/), then run the installer and follow the prompts.
- **MacOS**: Install Git using Homebrew by running `brew install git` in the terminal.
- **Linux**: Install Git from your package manager (for Ubuntu, run `sudo apt-get install git`).

## Configuring Git

After installation, set your user name and email address with these commands:

    git config --global user.name "Your Name"
    git ig config --global user.email "your.email@example.com"

## Creating a New Repository

To start a new project with Git, create a new directory, and initialize it with Git:

    mkdir myproject
    cd myprojects
    git init

## Cloning a Repository

To work on an existing project, you can clone its repository:

    git clone https://github.com/username/repository.git

## Basic Git Workflow

Here's a basic workflow for making changes to your project:

1. **Check Status**: See what changes are pending.

        git status

2. **Stage Changes**: Add files you want to include in your commit.

        git add filename

3. **Commit Changes**: Save your changes to the local repository.

        git commit -m "Commit message"

4. **Push Changes**: Upload your commit to a remote repository.

        git push origin main

## Branching

Branches are used to develop features isolated from each other:

1. **Create a Branch**: 

        git branch new-branch

2. **Switch to the Branch**: 

        git checkout new-branch
    Or, to create and switch to one step (including step 1):
        git checkout -b new-branch
    with -b is an option combined with `checkout` that tells Git to create a new branch.

3. **Merge the Branch**: First, switch back to the main branch, then merge.

        git checkout main
        git merge new-branch

## Pulling Changes

To update your local repository with the latest changes from remote:

    git pull origin main

## Conclusion

This guide covers the basic commands and workflows to get you started with Git. For more detailed information, refer to the official Git documentation at [git-scm.com/docs](https://git-scm.com/docs).
