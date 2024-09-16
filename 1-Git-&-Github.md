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
