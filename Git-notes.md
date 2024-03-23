
# Git for Absolute beginners
# Agenda 
- Module-01: What it git and its Benefits
- Module-02: Setting Up and Configuring Git
- Module-03: Key Components of a Git Repository
- Module-04: Understanding Git Workflow
- Module-05: Repository Status and Changes:
- Module-06: Git Operations: Clone, Pull, Fetch, Push, Merge
- Module-07: Exploring Branches and Merging
- Module-08: Stashing and Undoing Changes
- Module-09: Git Tags  -Purpose and Types
- Module-10: Collaboration and Advanced Operations
- Module-11: Inspection and Comparison
- Module-12: Debugging and Troubleshooting
- Module-13: Tips and Best Practices

  ----------------++++++-----------------
 # Module-01: What it git and its Benefits
Git is an open-source distributed version control system that allows developers to track changes in their codebase, collaborate with others, and manage software development projects effectively. It provides features such as branching, merging, and version history tracking, enabling developers to work on different features or fixes simultaneously while maintaining a complete history of their project's development. 
# Key benefits include:

- **Distributed Development**: Enables offline and independent work.
- **Data Integrity**: Ensures consistency and integrity of project data.
- **Branching and Merging**: Facilitates parallel work and seamless integration of changes.
- **Speed and Performance**: Operations like committing and merging are fast, even for large projects.
- **History Tracking**: Maintains a detailed history of changes for traceability and version control.
- **Collaboration**: Supports seamless sharing, reviewing, and collaboration among developers.
- **Flexible Workflow**: Adaptable to various workflow models to suit project needs.
- **Open Source and Community Support**: Benefits from a large community providing support and tools.
- **Security**: Implements security features to protect project data and ensure integrity.
- **Platform Independence**: Works across different operating systems, allowing collaboration across environments.

# Module-02: Setting Up and Configuring Git
To start using Git, follow these steps to set it up and configure it according to your preferences:
1. **Install Git**:
   - Download and install Git from [git-scm.com](https://git-scm.com/).
2. **Check Git Version**:
   - Open a terminal or command prompt and run the following command to check the Git version:
     ```
     git --version
     ```
3. **Configure User Information**:
   - Set up your username and email address using the following commands:
     ```
     git config --global user.name "Your Name"
     git config --global user.email "your.email@example.com"
     ```
     Replace "Your Name" with your actual name and "your.email@example.com" with your email address.

4. **Configure Credential Manager**:
   - Enable credential caching for HTTPS connections to avoid entering credentials repeatedly:
     ```
     git config --global credential.helper cache
     ```
5. **Check Configuration**:
   - Verify your Git configuration settings by running the following command:
     ```
     git config --list
     ```
Once Git is installed and configured successfully, congratulations! You are ready to start using it for version control in your projects. 
# Module-03: Key Components of Git Repository
A Git repository comprises:
1. **Working Directory**:
   - Local directory where files are edited.
   - Represents the current state of the project.
2. **Staging Area** (Index):
   - Prepares changes for commit.
   - Allows selective staging of modifications.
3. **Repository**:
   - Stores project history and metadata.
   - Centralized location for collaboration.
     
Understanding these components is essential for effective version control with Git.

<img width="466" alt="image" src="https://github.com/DevOps-Organization001/Git-for-Absolute-beginners/assets/128646718/5f99d68d-4dff-4582-acc5-07e04ede8450">

# Module-04: Understanding Git Workflow
A Git workflow is a series of steps that developers follow to manage their code and collaborate effectively using the Git version control system.

<img width="539" alt="image" src="https://github.com/DevOps-Organization001/Git-for-Absolute-beginners/assets/128646718/872b0eaf-3323-48a7-b4fe-368dc01ea924">

# Module-05: Repository Status and Changes:

Manage changes in your Git repository effectively using the following commands:

| Sl no | Command                                   | Description                                        | Example                            |
|-------|-------------------------------------------|----------------------------------------------------|------------------------------------|
| 1     | `git status`                              | Check repository status.                          | `git status`                       |
| 2     | `git add <file_name>`                     | Add changes to staging area.                      | `git add index.html`               |
| 3     | `git add .`                               | Add all changes to staging area.                  | `git add .`                        |
| 4     | `git reset`                               | Unstage changes from staging area.                | `git reset`                        |
| 5     | `git commit -m "Your commit message"`     | Commit changes with a message.                    | `git commit -m "Initial commit"`   |
| 6     | `git commit -a -m "Your commit message"`  | Stage and commit changes in one command.          | `git commit -a -m "Fix: a bug"`    |
| 7     | `git commit --amend -m "New commit message"` | Amend the last commit message.                 | `git commit --amend -m "Fix: another bug"` |
| 8     | `git log`                                 | View commit history.                              | `git log`                          |
| 9     | `git log --oneline`                       | View one-line commit history.                     | `git log --oneline`                |
| 10    | `git log --graph`                         | Visualize commit history as a graph.              | `git log --graph`                  |
| 11    | `git log --since="2 weeks ago"`           | Show commits within a time range.                 | `git log --since="2 weeks ago"`    |
| 12    | `git log --author="John Doe"`             | Show commits by a specific author.               | `git log --author="John Doe"`      |
| 13    | `git log --grep="keyword"`                | Search commits by a keyword.                      | `git log --grep="bug fix"`         |
| 14    | `git diff`                                | Show changes not yet staged.                      | `git diff`                         |
| 15    | `git diff --staged`                       | Show changes in the staging area.                 | `git diff --staged`                |
| 16    | `git diff <commit_hash>`                  | Show changes between current and specified commit. | `git diff abc123`                  |
| 17    | `git diff <branch_name>`                  | Show changes between current and specified branch. | `git diff main feature-branch`     |
| 18    | `git blame <file_name>`                   | Show last modifier of each line in a file.        | `git blame index.html`             |

Use these commands to track changes, commit revisions, and manage your Git repository efficiently.
# Module-06: Git Operations: Clone, Pull, Fetch, Push, Merge
## Clone
- **Definition**: Creates a local copy of a repository.
- **Usage**: `git clone <repository_url>`
## Pull
- **Definition**: Updates the local branch with remote changes.
- **Usage**: `git pull`
## Fetch
- **Definition**: Retrieves remote changes without merging.
- **Usage**: `git fetch`
## Push
- **Definition**: Sends local commits to the remote repository.
- **Usage**: `git push`
## Merge
- **Definition**: Combines changes from different branches.
- **Usage**: `git merge <branch_name>`
These operations are fundamental for collaborating on Git projects and updating repositories.
![image](https://github.com/DevOps-Organization001/Git-for-Absolute-beginners/assets/128646718/1d9f6ed2-d37d-4791-9faa-6331ad73daf2)

# Module-07: Exploring Branches and Merging

## Branch
- **Definition**: 
  - A branch in Git represents a separate line of development within a repository. It allows developers to work on features or fixes without directly altering the main codebase. Think of it as a parallel universe where changes can be made independently.
    
## Merging Strategies in Git
- Merging strategies in Git determine how changes from different branches are combined into a single branch. There are three main merging strategies in Git:
  
### 1. Rebase:
- **Definition**:
  - Rebase is a merging strategy that rewrites the commit history by moving all the commits of one branch onto another. This creates a cleaner and more linear history but can be risky if used incorrectly.
- **Pros**:
  - Results in a cleaner commit history without merge commits cluttering the timeline.
- **Cons**:
  - Can cause conflicts if multiple developers are working on the same branch.
  - Should be used cautiously to avoid losing commits or causing confusion in collaborative environments.

### 2. Fast-forward Merge:
- **Definition**:
  - Fast-forward merge is the simplest merging strategy where Git simply moves the pointer of the current branch to the latest commit of the branch being merged. This strategy is efficient but can lead to a messy history with multiple parallel branches.
- **Pros**:
  - Results in a straightforward linear history.
  - Fast and efficient.
- **Cons**:
  - History can become cluttered with parallel branches and lacks clear separation between features.

### 3. Three-way Merge:
- **Definition**:
  - Three-way merge is a strategy that considers the common ancestor of the branches being merged, the changes made on both branches, and resolves any conflicts that arise. This strategy ensures a clear history and handles conflicts effectively.
- **Pros**:
  - Handles conflicts gracefully, ensuring that changes are integrated smoothly.
  - Results in a clear and structured commit history.
- **Cons**:
  - More complex than fast-forward merges and may require manual intervention to resolve conflicts.

These merging strategies offer different trade-offs in terms of simplicity, efficiency, and clarity of history. Choosing the right strategy depends on the specific requirements and workflow of your project.

# Choosing the right Git strategy based on:
- Team workflow
- History clarity
- Risk tolerance

# Git Branching and Merging Commands

| Sl no | Command                                      | Description                                            | Example                                      |
|-------|----------------------------------------------|--------------------------------------------------------|----------------------------------------------|
| 1     | `git branch`                                 | List all local branches.                               | `git branch`                                 |
| 2     | `git branch -a`                              | List all local and remote branches.                   | `git branch -a`                              |
| 3     | `git branch <branch_name>`                   | Create a new branch.                                   | `git branch feature-branch`                  |
| 4     | `git branch -m <old_branch_name> <new_branch_name>` | Rename a local branch.                          | `git branch -m old-feature new-feature`     |
| 5     | `git branch -d <branch_name>`                 | Delete a local branch.                                 | `git branch -d feature-branch`              |
| 6     | `git branch -D <branch_name>`                 | Force delete a local branch.                           | `git branch -D feature-branch`              |
| 7     | `git checkout -b <new_branch_name>`           | Create and switch to a new branch.                     | `git checkout -b new-feature`               |
| 8     | `git checkout <branch_name>`                  | Switch to a branch.                                    | `git checkout feature-branch`               |
| 9     | `git merge <branch_name>`                     | Merge a branch into the current branch.                | `git merge feature-branch`                  |
| 10    | `git merge --no-ff <branch_name>`             | Merge with a new commit, not fast-forward.             | `git merge --no-ff feature-branch`          |
| 11    | `git rebase <branch_name>`                    | Rebase the current branch onto another branch.         | `git rebase main`                           |
| 12    | `git rebase --abort`                          | Abort a rebase.                                        | `git rebase --abort`                        |
| 13    | `git rebase --continue`                       | Continue a rebase after resolving conflicts.           | `git rebase --continue`                     |
| 14    | `git rebase -i HEAD~n`                        | Interactive rebase.                                    | `git rebase -i HEAD~3`                      |
| 15    | `git cherry-pick <commit_hash>`               | Cherry-pick a commit.                                  | `git cherry-pick abc123`                    |
| 16    | `git revert <commit_hash>`                    | Revert a commit.                                       | `git revert abc123`                         |
| 17    | `git revert -n <commit_hash>`                 | Revert a commit without committing immediately.        | `git revert -n abc123`                      |
| 18    | `git branch --set-upstream-to=origin/<remote_branch_name> <local_branch_name>` | Set the upstream branch.            | `git branch --set-upstream-to=origin/main main` |

These commands are essential for managing branches, merging changes, and maintaining a structured Git workflow.

# Module-08: Stashing and Undoing Changes

| Sl no | Command                                      | Description                                            | Example                                      |
|-------|----------------------------------------------|--------------------------------------------------------|----------------------------------------------|
| 1     | `git stash`                                  | Stash changes.                                         | `git stash`                                  |
| 2     | `git stash apply`                            | Apply stashed changes.                                 | `git stash apply`                            |
| 3     | `git stash pop`                              | Apply and drop the latest stash.                       | `git stash pop`                              |
| 4     | `git stash list`                             | List stashes.                                          | `git stash list`                             |
| 5     | `git stash show`                             | Show changes in the latest stash.                      | `git stash show`                             |
| 6     | `git stash drop`                             | Delete the latest stash.                               | `git stash drop`                             |
| 7     | `git stash drop <stash_id>`                  | Delete a specific stash.                               | `git stash drop 2`                           |
| 8     | `git stash clear`                            | Delete all stashes.                                    | `git stash clear`                            |
| 9     | `git rm <file_name>`                         | Remove a file from the repository.                     | `git rm old_file.txt`                        |
| 10    | `git rm --cached <file_name>`                | Untrack a file but keep it in the working directory.   | `git rm --cached sensitive_info.txt`        |
| 11    | `git mv <old_file_name> <new_file_name>`    | Rename or move a file.                                 | `git mv old_name.txt new_name.txt`          |
| 12    | `git checkout -- <file_name>`                | Undo changes in the working directory.                 | `git checkout -- file.txt`                  |
| 13    | `git reset HEAD~1`                          | Undo the last commit (local).                          | `git reset HEAD~1`                          |
| 14    | `git restore <file_name>`                    | Discard local changes.                                 | `git restore file.txt`                       |
| 15    | `git clean -n`                               | Show untracked files that will be deleted.             | `git clean -n`                               |
| 16    | `git clean -f`                               | Delete untracked files.                                | `git clean -f`                               |

These commands are essential for stashing changes, undoing modifications, and maintaining a clean Git repository.

# Module-09: Git Tags  -Purpose and Types
## Purpose of Git Tags
- A Git tag serves as a marker for a specific point in your project's history.
- It is commonly used for marking releases and important milestones.
- Tags are essential for versioning and release management.

## Types of Git Tags
- There are two main types of Git tags, each suited for different
situations:
1. Lightweight Tags:
   - Lightweight tags are simply pointers to specific commits.
   - They are created using the `git tag` command without additional metadata.

2. Annotated Tags:
   - Annotated tags are like commits, with additional metadata such as tagger name, email, date, and a tagging message.
   - They are created using the `-a` or `--annotate` option with the `git tag` command.

Use Git tags to mark significant points in your project's history, aiding in versioning and release management.

# Git Tags Commands

| Sl no | Command                                      | Description                                            | Example                                      |
|-------|----------------------------------------------|--------------------------------------------------------|----------------------------------------------|
| 1     | `git tag`                                    | List all tags.                                         | `git tag`                                    |
| 2     | `git tag -a <tag_name> -m "Tag message"`    | Create an annotated tag.                              | `git tag -a v1.0 -m "Version 1.0"`          |
| 3     | `git tag -d <tag_name>`                      | Delete a tag.                                          | `git tag -d v1.0`                           |
| 4     | `git show <tag_name>`                        | Show information about a tag.                         | `git show v1.0`                             |
| 5     | `git push origin <tag_name>`                 | Push a specific tag to a remote repository.           | `git push origin v1.0`                      |
| 6     | `git push origin --tags`                     | Push all tags to a remote repository.                 | `git push origin --tags`                    |
| 7     | `git tag -l "v1.*"`                          | List tags matching a pattern.                         | `git tag -l "v1.*"`                         |
| 8     | `git describe <commit_hash>`                 | Show the most recent tag reachable from a commit.     | `git describe abc123`                       |
| 9     | `git tag -a <tag_name> <commit_hash> -m "Tag message"` | Create an annotated tag for a specific commit. | `git tag -a v1.1 abc123 -m "Version 1.1"` |
| 10    | `git tag -v <tag_name>`                      | Verify the signature of a tag.                        | `git tag -v v1.0`                           |
| 11    | `git tag -n`                                 | Show the annotation message for each tag.            | `git tag -n`                                |
| 12    | `git tag -a <tag_name> -f <commit_hash> -m "Updated tag message"` | Move or update an existing tag to a new commit. | `git tag -a v1.0 -f abc456 -m "Updated version 1.0"` |
| 13    | `git tag -d $(git tag -l "v1.*")`            | Delete tags matching a pattern.                       | `git tag -d $(git tag -l "v1.*")`           |
| 14    | `git push origin :<tag_name>`                | Delete a remote tag.                                  | `git push origin :v1.0`                     |
| 15    | `git fetch --tags`                          | Fetch tags from a remote repository.                  | `git fetch --tags`                          |
| 16    | `git tag -a <tag_name> -m "Tag message" <commit_hash>` | Create a tag for a specific commit.           | `git tag -a v1.2 -m "Version 1.2" abc789`  |

These commands are essential for managing Git tags, including creation, deletion, pushing, and fetching tags from remote repositories.
# Module-10: Collaboration and Advanced Operations

| Sl no | Command                                       | Description                                               | Example                                                 |
|-------|-----------------------------------------------|-----------------------------------------------------------|---------------------------------------------------------|
| 1     | `git remote`                                  | List remote repositories.                                 | `git remote`                                            |
| 2     | `git remote -v`                               | View remote repository URLs.                              | `git remote -v`                                         |
| 3     | `git remote show <remote_name>`               | Show information about a remote.                          | `git remote show origin`                                |
| 4     | `git remote add <remote_name> <remote_url>`   | Add a new remote repository.                              | `git remote add upstream https://github.com/upstream/repo.git` |
| 5     | `git remote remove <remote_name>`             | Remove a remote repository.                               | `git remote remove origin`                              |
| 6     | `git fetch`                                   | Fetch changes from remote.                                | `git fetch`                                             |
| 7     | `git pull origin <branch_name>`               | Pull changes from a remote repository.                    | `git pull origin main`                                  |
| 8     | `git push origin <branch_name>`               | Push changes to a remote repository.                      | `git push origin feature-branch`                        |
| 9     | `git push origin --delete <branch_name>`      | Delete a remote branch.                                   | `git push origin --delete feature-branch`               |
| 10    | `git fetch --prune`                           | Remove remote tracking branches that have been deleted.   | `git fetch --prune`                                     |
| 11    | `git branch -r --merged`                      | Show remote branches merged into the current branch.      | `git branch -r --merged`                               |
| 12    | `git branch -r --no-merged`                   | Show remote branches not yet merged into the current branch. | `git branch -r --no-merged`                            |
| 13    | `git push origin --all --force`               | Force-push all branches to a remote repository.          | `git push origin --all --force`                         |
| 14    | `git push origin --tags --force`              | Force-push tags to a remote repository.                  | `git push origin --tags --force`                        |
| 15    | `git fetch --all`                             | Fetch changes from all remotes.                           | `git fetch --all`                                       |
| 16    | `git reflog`                                  | Show a log of all changes, including branch deletions.   | `git reflog`                                            |
| 17    | `git fsck --full`                             | Check the repository for errors.                         | `git fsck --full`                                       |
| 18    | `git gc`                                      | Run Git garbage collection.                              | `git gc`                                                |
| 19    | `git archive --format=zip --output=latest.zip HEAD` | Create a zip archive of the latest commit.            | `git archive --format=zip --output=latest.zip HEAD`      |
| 20    | `git submodule add <repository_url>`          | Add a submodule to the repository.                        | `git submodule add https://github.com/example/submodule.git` |
| 21    | `git submodule update --init --recursive`     | Initialize and update submodules.                         | `git submodule update --init --recursive`               |
| 22    | `git submodule foreach git pull origin main`   | Update all submodules to the latest commit.               | `git submodule foreach git pull origin main`            |
| 23    | `git blame -L 10,20 <file_name>`              | Show the last modification to specific lines in a file.  | `git blame -L 10,20 index.html`                         |
| 24    | `git cherry <branch1> <branch2>`              | Show commits present in one branch but not in another.    | `git cherry main feature-branch`                        |
| 25    | `git log --since="2 weeks ago" --pretty=format:"%h - %an, %ar : %s"` | Show commits within a time range with a custom format. | `git log --since="2 weeks ago" --pretty=format:"%h - %an, %ar : %s"` |

# Module-11: Inspection and Comparison

Git provides several commands for inspecting and comparing changes in your repository:

| Sl no | Command                    | Description                                                  | Example                                   |
|-------|----------------------------|--------------------------------------------------------------|-------------------------------------------|
| 1     | `git status`               | Check current repository status.                             | `git status`                              |
| 2     | `git diff`                 | Show changes between working directory and index.            | `git diff`                                |
| 3     | `git log`                  | Display commit history.                                      | `git log`                                 |
| 4     | `git show <commit>`        | Display detailed information about a specific commit.        | `git show abc123`                         |
| 5     | `git reflog`               | Show a log of all reference updates.                         | `git reflog`                              |
| 6     | `git bisect`               | Find the commit that introduced a bug.                       | `git bisect start`                        |
| 7     | `git fsck`                 | Check the integrity of the Git objects database.             | `git fsck`                                |
| 8     | `git cat-file -p <object>` | Display the contents of a Git object.                        | `git cat-file -p abc123`                  |
| 9     | `git stash`                | Stash changes temporarily.                                  | `git stash`                               |
| 10    | `git cherry-pick <commit>` | Apply changes from a specific commit to the current branch. | `git cherry-pick abc123`                  |
| 11    | `git checkout -- <file>`   | Discard changes in the working directory for a file.        | `git checkout -- file.txt`                |
| 12    | `git reset --hard HEAD~1`  | Reset the current branch to the previous commit.            | `git reset --hard HEAD~1`                 |
| 13    | `git revert <commit>`      | Revert specific commits, creating a new commit.             | `git revert abc123`                       |
| 14    | `git clean -n`             | Show untracked files that will be deleted.                  | `git clean -n`                            |

# Module-12: Debugging and Troubleshooting

Additionally, Git offers tools for debugging and troubleshooting issues in your repository:

| Sl no | Command                    | Description                                                  | Example                                   |
|-------|----------------------------|--------------------------------------------------------------|-------------------------------------------|
| 1     | `git bisect`               | Find the commit that introduced a bug.                       | `git bisect start`                        |
| 2     | `git fsck`                 | Check the integrity of the Git objects database.             | `git fsck`                                |
| 3     | `git reflog`               | Show a log of all reference updates.                         | `git reflog`                              |
| 4     | `git stash`                | Stash changes temporarily.                                  | `git stash`                               |
| 5     | `git cherry-pick <commit>` | Apply changes from a specific commit to the current branch. | `git cherry-pick abc123`                  |
| 6     | `git revert <commit>`      | Revert specific commits, creating a new commit.             | `git revert abc123`                       |
| 7     | `git grep <pattern>`       | Search for a specific text pattern in the codebase.         | `git grep "functionName"`                  |
| 8     | `git blame <file>`         | Display the author and revision information of a file.      | `git blame index.html`                    |
| 9     | `git clean -n`             | Show untracked files that will be deleted.                  | `git clean -n`                            |
| 10    | `git log --oneline`       | Show commit history in a compact format.                    | `git log --oneline`                       |

These commands are essential for identifying and resolving issues in your Git repository

# Module13: Tips and Best Practices
When working with Git, consider the following tips and best practices:

- **Commit frequently:** Make small, focused commits to track changes effectively and make it easier to understand the history of your project.

- **Utilize branches:** Use branches to work on new features or bug fixes without affecting the main codebase. This allows for parallel development and easier collaboration.

- **Test early and often:** Test your changes regularly to catch issues early in the development process. This helps prevent bugs from being introduced into the codebase.

- **Backup your work:** Regularly push your changes to a remote repository to ensure that your work is backed up and accessible from multiple locations.

- **Seek help if needed:** Don't hesitate to reach out to colleagues, online forums, or documentation if you encounter difficulties or have questions about Git. Collaboration and knowledge sharing can help resolve issues more efficiently.

These practices can help streamline your workflow, improve collaboration, and ensure the stability of your projects.

**Hey there,**
**If you found this content helpful, please consider 🔔 Subscribing to our [Azure DevOps Pulse](https://www.youtube.com/@AzureDevOpsPulse) Youtube channel for more!**

# Happy learning!  
 Cheers,  
 Hriyen
