# 📌 Working with repositories.
So, what can we do with repositories? We can create (initialize), import (clone), modify or delete a repository.  

## 🔹 Creating or importing repositories.  
To start working with a repository, you need to either initialize a new local repository or clone an existing one from a remote source (origin).  
To initialize a repository locally we must use the `git init` command, and to clone a remote repository we use the `git clone` command.

### ▫️ Git init
Git init is the command that initializes a new empty repository on your local working directory. This command will create a new repository without any files in it aside from [**.git/**](#the-git-directory) directory.

**Syntax**
```bash
git init name-of-repo
```   

**Example**
```bash
git init myFirstRepo
```
This command creates a new repository named myFirstRepo without any upstream syncronization or connection.

### ▫️ Git clone
Git clone is used to create a local copy of an existing Git repository. This command downloads the repository, including all its files, commit history, branches, and tags, to your local machine.
By default, it also sets the remote repository (referred to as origin) as the upstream, so you can easily push changes back to the original repository after committing them locally.
**Syntax**
```bash
git clone link-to-source-repository
```   

**Example**
```bash
git clone https://github.com/user/repository.git
```
This command creates a new directory named after the repository (unless specified otherwise) and clones all its contents into that directory.
   
   
> [!IMPORTANT]
> Using **git init** no [upstream connection](#upstream-reference) will be configured and you will have to do that manually.

## 🔹 Modifying a repository.
Within a repository you can perform several actions.
- Rename the repository.
- Change the default branch.
- Modify repository visibility (public/private).
- Manage collaborators and permissions.
- Set up webhooks or branch protection rules.
- Enable or disable features like issues or wikis.

## 🔹 Deleting a repository.



## 🔹 What defines a git repository in our system.
A repository is characterized by a series of files and subdirectories located in the [**.git/**](#the-git-directory) directory. These files are essential for managing various aspects of your repository, including branch tracking, [upstream connections](#upstream-reference), local repository history, and references.

> [!CAUTION]
> Deleting any of these files can lead to significant harm and potentially irreversible data loss if your work has not been pushed to a remote repository.

---

## 🔹 Working with git areas.
