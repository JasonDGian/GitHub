
--- 
   
# Welcome to my Git and GitHub explanation repo.
In this repository, I will compile my knowledge about **Git** and **GitHub** to create a comprehensive reference for anyone needing a quick guide—a detailed cheat sheet for newcomers. The idea originated from a good friend who asked for tips about these tools, and I thought it would be beneficial for both of us to document this information. 

>[!Note]
>If you are willing to contribute to improving and expanding this humble guide, by all means, go ahead! Your contributions are welcome.

**Without further ado, let's jump in.**
   
--- 

# Git & GitHub - Know the difference.
Before we begin, I'd like to make the somewhat pedantic distinction between Git and GitHub. 
- Git is the version control system you install on your device (computer).
- GitHub is the web-based platform where you can store and manage your Git repositories.
   
Git is a versatile tool that can be used not only with GitHub but also in a variety of other configurations. For example, a company might manage its codebase through a strictly local repository, allowing employees to collaborate internally without relying on an external hub. Similarly, a solo developer might use Git solely on their own PC for personal projects, choosing not to upload their files to any external service. 

> [!IMPORTANT]
> To use Git, you'll need to install it on your system. The installation process varies depending on your operating system and distribution; whether you're using Linux or Windows. But you probably already knew that.

---

# Git and Github - File areas
Git and Github manage files by putting them in four separate 'areas'. It is important to understand these areas so not to cause any trouble when working with repositories. There are 4 areas in which the files of your code can reside. 

![book](https://github.com/user-attachments/assets/48145eed-e5bc-400e-a194-9846997c761b)

1. Working directory.
2. Staging area.
3. Local repository.
4. Remote repository.

### Git - Working directory.
The working directory is the local folder where all your files are stored while you work on them.

### Git - Staging area.
The staging area is a temporary space. This is where the files you want to save and send to the local repository are placed before you confirm your action.

### Git - Local repository.
The local repository exists on your machine and is not connected to the internet. If you lose your machine, or delete the root folder, you will also lose this repository.

### GitHub - Remote repository.
The remote repository, often referred to as 'origin', is synchronized with your local repository to save and share your work.
<br/>

#### The typical workflow of Git + GitHub:
   
1. **Make Changes** - Modify files in your working directory.
2. **Stage Changes** - Add the modified files to the staging area.
3. **Commit Changes** - Save the changes to your local repository with a descriptive message.
4. **Push Changes** - Synchronize your local repository with the remote repository (origin) by pushing the committed changes.

---

# Working with repositories.
To work with a repository, you need to either initialize a new local repository or clone an existing one from a remote source (origin).

To initialize a repository locally we must use the `git init <new_repo_name> ` command, and to clone a remote repository we use the `git clone <existing_repo_link>` command.

## Git init
Git init is the command that initializes a new empty repository on your local working directory. This command will create a new repository without any files in it aside from [**.git/**](#the-git-directory) directory.
`git init name-of-repo`   

## Git clone
Git clone is used to create a copy of an existing Git repository. When you clone a repository, you create a new local repository that is an exact duplicate of the remote repository, including all its history and branches.   
`git clone link-to-source-repository`

> [!IMPORTANT]
> Using **git init** no [upstream connection](#upstream-reference) will be configured and you will have to do that manually.


## What defines a git repository in our system.
A repository is characterized by a series of files and subdirectories located in the [**.git/**](#the-git-directory) directory. These files are essential for managing various aspects of your repository, including branch tracking, [upstream connections](#upstream-reference), local repository history, and references.

> [!CAUTION]
> Deleting any of these files can lead to significant harm and potentially irreversible data loss if your work has not been pushed to a remote repository.

---

## Working with git areas.



---

# TODO
The following concepts will be here documented and elucidated.

# Branches
## Main
## Feature
## Develop
## Testing

# Tags


## Areas.

# Working directory.
# Staging area.
# Remote repository.

# Head
# Detached head
# Upstream
# Origin


`git remove cached` -> mirar correcto.
`git init` - Initializes a new local repository.
  
`git clone` - Clones a repository from a remote source.

`git fetch` - Downloads the latest information on commits, branches etc.. for the current repository.

`git pull` - 'Pulls' the changes present in the remote repository to your local repository.

`git push` - Uploads the changes currently staged to the remote repository.

`git status`

`git add`

`git commit`
`git alias`
`git merge`
`git branch`
`git checkout`
`git clean`
`git config`
`git log`
`git rebase`
`git stash`


# Other notes.

## The .git/ directory.
This directory contains the files that are used to track and keep record of your repository. **Deleting this directory will efectively destroy the repository status.** 

## Upstream reference.
The **upstream flow** or **upstream reference** is the link that connects your local repository on your machine with the remote repository on GitHub. This connection ensures that changes in your local repository can be pushed to the remote repository. Without this link, Git would have no way to transmit your local changes to the remote repository, as it wouldn't know where to send them.

To set an upstream flow use command: 
`git branch --set-upstream <remote-repository>`

----

1. Introduction to Version Control

    What is version control?
    Benefits of using version control systems

2. Basic Git Concepts

    What is Git?
    Local repository vs. remote repository
    Git's architecture: Working directory, staging area, and local repository

3. Setting Up Git

    Installing Git
    Basic configuration (git config)

4. Creating and Cloning Repositories

    Initializing a new repository (git init)
    Cloning an existing repository (git clone)

5. Basic Git Workflow

    Checking the status of the repository (git status)
    Adding changes to the staging area (git add)
    Committing changes (git commit)
    Viewing commit history (git log)

6. Branching and Merging

    What is a branch?
    Creating and switching branches (git branch, git checkout)
    Merging branches (git merge)
    Resolving merge conflicts

7. Remote Repositories

    What is a remote repository?
    Adding and managing remote repositories (git remote)
    Fetching and pulling changes (git fetch, git pull)
    Pushing changes (git push)

8. Tagging

    What are tags?
    Creating and listing tags (git tag)

9. Undoing Changes

    Viewing changes (git diff)
    Undoing changes in the working directory (git checkout, git restore)
    Removing changes from the staging area (git reset)
    Reverting commits (git revert)

10. Advanced Git Commands

    Interactive rebase (git rebase -i)
    Cherry-picking commits (git cherry-pick)
    Stashing changes (git stash)

11. GitHub Basics

    What is GitHub?
    Creating a GitHub account
    Navigating the GitHub interface
    Forking repositories
    Creating pull requests

12. Collaborative Workflow

    Forking and contributing to projects
    Using issues and project boards
    Code reviews and collaboration best practices

13. GitHub Actions and Automation

    Introduction to GitHub Actions
    Setting up workflows for continuous integration (CI) and continuous deployment (CD)

14. Advanced GitHub Features

    GitHub Pages for project documentation
    Managing repository settings and permissions
    Leveraging GitHub’s API and integrations
