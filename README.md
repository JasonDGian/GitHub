
 <H1 style="color:red;">WARNING</H1>
 
> THIS IS A WORK IN PROGRESS DOC.   
> Information and concepts are not in the final order.   
> Some concepts are missing.   
> Some nasty drafts are currently written down.   
> Most of this document will change and improve in the future.   

--- 
   
# Welcome to my Git and GitHub explanation repo.
In this repository, I will compile my knowledge about **Git** and **GitHub** to create a comprehensive reference for anyone needing a quick guide, sort of a detailed cheat sheet for newcomers. The idea originated from a good friend who asked for tips about these tools, and I thought it would be beneficial for both of us to document this information. In case you are looking for the, much more detailed, official docs check [here!](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories)

>[!Note]
>If you are willing to contribute to improving and expanding this humble guide, by all means, go ahead! Your contributions are welcome.

**Without further ado, let's jump in.**
   
--- 




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


<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>



Provided that the remote repository is origin, and that you're interested in master:

git fetch origin
git reset --hard origin/master







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



# OPERACIONES.

Crear un repositorio.
  - Inicializar un repositorio.
    - Sincronizar flujo de subida.
  - Clonar un repositorio.
  - Bifurcar (fork) un repositorio.

Renombrar un repositorio.

Cambios en los repositorios.
  Actualizar cabeceras.
  Descargar cambios desde remoto.
  Subir cambios de local a remoto.

Re-escribir la historia de un repositorio.
  - Reescribir la historia local.
  - Reecribir la historia remota.

Administrar ramas.
- Crear una rama.
- Fusionar una rama (merge).


# Borrar ficheros en GitHub.
Para borrar ficheros del repositorio remoto usamos el siguiente comando (esto no afectará los ficheros presentes en el directorio de trabajo local).
```git
git rm -r --cached
```

Tambien podemos hacerlo tomando como referencia nuestro directorio de trabajo local. De este modo, todos los ficheros que borramos en el directorio de trabajo local desaparecerán también del repositorio remoto.
```git
git commit -a
```
https://git-scm.com/docs/git-rm
