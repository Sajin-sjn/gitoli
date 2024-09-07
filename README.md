# gitoli
1. Create a repository in github.

2. Open a directory in vs code where you want to create the project folder having git.

3. Navigate to the terminal, 
```bash
    git clone "your repo web url"
```
⇒ cloning
    - You create a local copy of the project from a remote repository (e.g., GitHub, GitLab). This allows you to work on the project    files locally.

4. Open the terminal and enter
```bash
    git status
```
⇒ command explanation
    - The command git status shows the current state of your Git repository

5. Now the files are tracked by the git, When you modify a file in the cloned repository, Git detects that the file has been changed. The file's status changes from "unmodified" to "modified," meaning the file is different from its version in the repository.

6. You should stop your modifications and add changes to staging when you reach a logical point in your work. 
    - Completed a meaningful task
    - Before switching tasks
    - After testing
    - Small incremental steps

7. Afer the successfull modifications , execute 
```bash
    git add .
```
⇒ command explanation
    - When you modify files, they are in your working directory. git add moves these changes to the staging area, where you prepare them for committing.

8. After staging the modifications by executing the above command , execute
```bash
    git commit -m "Describe what changes were made"
```
⇒ command explanation
    - Commits or records the staged files with a descriptive message explaining the changes. Each commit creates a snapshot of the project at a specific point in time.

9. The changes are recorded in your local repository. If you want to mark your changes in your remote repo, need to execute
```bash
    git push origin main
```
    - After executing this command,
        - Local Commits Are Uploaded
        - Remote Repository Updates
        - Your local main branch will now be synchronized with the remote main branch
        - Your changes become visible to other collaborators who have access to the remote repository

⇒ Theses are all the major steps you have to take to start your project on local repo and push the changes to remote repo


## Maximum effort
```bash
    git add -am "your commit message"
```
This command used to stage all changes to tracked files and commit them in one step

- NB : If you need to include new files or deletions, you should use git add first, followed by git commit

---

```bash
    git pull origin main
```
Fetches new data from the remote repository and immediately merges it into your current branch.

---

```bash
    git remote add origin <remote_repository_URL>
```
- **git remote add :** This part of the command is used to add a new remote repository to your local Git repository.
- **origin :** This is the name you’re giving to the remote repository. By convention, origin is the default name used for the main remote repository, but you can name it anything you like.
- **<remote_repository_URL>:**  This is the URL of the remote repository where you want to push your code. This URL can be an HTTPS URL, an SSH URL, or another supported URL format.


