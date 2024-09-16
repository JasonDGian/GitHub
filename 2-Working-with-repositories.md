# 📌 Working with repositories.
So, what can we do with repositories? We can create (initialize), import (clone), modify or delete a repository.  

## 🔹 Creating or importing repositories.  
To start working with a repository, you need to either initialize a new local repository or clone an existing one from a remote source (origin).  
To initialize a repository locally we must use the `git init <new_repo_name> ` command, and to clone a remote repository we use the `git clone <existing_repo_link>` command.

### ▫️ Git init
Git init is the command that initializes a new empty repository on your local working directory. This command will create a new repository without any files in it aside from [**.git/**](#the-git-directory) directory.
`git init name-of-repo`   

### ▫️ Git clone
Git clone is used to create a copy of an existing Git repository. When you clone a repository, you create a new local repository that is an exact duplicate of the remote repository, including all its history and branches.   
`git clone link-to-source-repository`

> [!IMPORTANT]
> Using **git init** no [upstream connection](#upstream-reference) will be configured and you will have to do that manually.

## 🔹 Modifying a repository.

## 🔹 Deleting a repository.



## 🔹 What defines a git repository in our system.
A repository is characterized by a series of files and subdirectories located in the [**.git/**](#the-git-directory) directory. These files are essential for managing various aspects of your repository, including branch tracking, [upstream connections](#upstream-reference), local repository history, and references.

> [!CAUTION]
> Deleting any of these files can lead to significant harm and potentially irreversible data loss if your work has not been pushed to a remote repository.

---

## 🔹 Working with git areas.
