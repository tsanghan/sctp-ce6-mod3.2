# sctp-ce6-mod3.2

### 1. What is GitHub Authentication?

GitHub Authentication is the process of verifying your identity when accessing GitHub resources like repositories, issues, and pull requests. Authentication is crucial for maintaining security and ensuring that only authorized users can access or modify a repository. It can be implemented using various methods, allowing users to choose the one that best fits their needs.

**Methods of GitHub Authentication:**

1. **Password Authentication:**
   - *Deprecated*: Password-based authentication for Git operations has been removed in favor of more secure methods.

2. **Personal Access Tokens (PAT):**
   - A personal access token works like a password for GitHub. It grants access to specific repositories and scopes that you define. This is more secure than using a password because you can restrict the scope of access and revoke the token if it’s compromised.

3. **SSH Keys:**
   - SSH keys are cryptographic keys that provide a secure way to authenticate with GitHub without using a password. You generate a public/private key pair, upload the public key to GitHub, and use the private key on your local machine to authenticate.

4. **OAuth Tokens:**
   - OAuth tokens allow third-party applications to interact with your GitHub account securely. When you authenticate using OAuth, you’re granting an application specific permissions to act on your behalf.

5. **GitHub App Installation Access Tokens:**
   - GitHub Apps authenticate using installation access tokens, which are generated for specific GitHub App installations. These tokens provide the GitHub App with a temporary and limited ability to act on your behalf.

6. **Web Authentication via Browser:**
   - When accessing GitHub via the web interface, authentication is typically done using a combination of username/password and two-factor authentication (2FA). You can also use Single Sign-On (SSO) for enterprise accounts.

### 2. List of 15 Git Commands and Their Usage

1. **`git init`**:
   - Initializes a new Git repository in the current directory.

2. **`git clone <repository>`**:
   - Clones an existing Git repository from a remote server to your local machine.

3. **`git status`**:
   - Shows the status of your working directory and staging area, displaying changes that have been staged, unstaged, or not tracked.

4. **`git add <file>`**:
   - Adds specific files or changes in files to the staging area for the next commit.

5. **`git commit -m "message"`**:
   - Records changes to the repository with a descriptive message.

6. **`git push origin <branch>`**:
   - Pushes changes from the local branch to the remote repository.

7. **`git pull origin <branch>`**:
   - Fetches changes from the remote repository and merges them into the current branch.

8. **`git branch`**:
   - Lists, creates, or deletes branches. Without any arguments, it lists all the branches in the repository.

9. **`git checkout <branch>`**:
   - Switches to a different branch or restores files to a specific state.

10. **`git merge <branch>`**:
    - Merges changes from one branch into the current branch.

11. **`git log`**:
    - Shows the commit history for the current branch.

12. **`git remote`**:
    - Manages connections to remote repositories, allowing you to add, remove, or modify remotes.

13. **`git fetch`**:
    - Downloads objects and refs from another repository but does not merge them automatically.

14. **`git rebase <branch>`**:
    - Reapplies commits on top of another base branch. Often used to clean up commit history.

15. **`git stash`**:
    - Temporarily saves changes that are not yet ready to be committed so you can work on something else and come back later.

### 3. The 4 Most Used Git Commands in Real-World Projects

1. **`git clone`**:
   - **Usage**: This command is commonly used when you first start working on a project. It allows you to copy a repository from a remote server to your local machine, so you can work on it locally.
   - **Real-World Scenario**: Developers often use `git clone` to get a copy of the project repository on their local machines when joining a new project or setting up a new development environment.

2. **`git commit`**:
   - **Usage**: The `git commit` command is essential for recording changes to the repository. It creates a new snapshot of the changes made to the files in the repository.
   - **Real-World Scenario**: Every time a developer makes a meaningful change, whether fixing a bug, adding a new feature, or refactoring code, they use `git commit` to save those changes in the project’s history.

3. **`git push`**:
   - **Usage**: This command is used to upload local repository content to a remote repository. It’s how you share your changes with others on the project.
   - **Real-World Scenario**: After making and committing changes, developers push their code to the remote repository so that it can be reviewed, merged, and deployed. This is crucial for collaborative development.

4. **`git pull`**:
   - **Usage**: The `git pull` command is used to fetch and merge changes from the remote repository into your current branch. It ensures that your local copy of the repository is up to date with the latest changes.
   - **Real-World Scenario**: Before starting new work or committing new changes, developers often pull the latest changes from the remote repository to avoid conflicts and ensure they are working with the most current version of the code.