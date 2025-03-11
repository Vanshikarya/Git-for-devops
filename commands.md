Git Commands

1. Initialization
   Initialize a new Git repository:
   git init

2. Configuration
   Set global username:
   git config --global user.name "Your Name"

   Set global email:
   git config --global user.email "your-email@example.com"

   Check configured settings:
   git config --list

3. File Operations
   Create a new file:
   touch <filename>

   Remove a file:
   rm <filename>

   Restore a deleted file:
   git restore <filename>

   Move or rename a file:
   git mv <old_filename> <new_filename>

4. Staging and Commit
   Check repository status:
   git status

   Add a file to staging:
   git add <filename>

   Add all files to staging:
   git add .

   Commit changes with a message:
   git commit -m "your commit message"

   Amend the last commit:
   git commit --amend -m "new commit message"

5. Branching
   Create a new branch:
   git branch <branch_name>

   Switch between branches:
   git checkout <branch_name>

   Create and switch to a new branch:
   git checkout -b <branch_name>

   List all branches:
   git branch

   Delete a branch:
   git branch -d <branch_name>

   Force delete a branch:
   git branch -D <branch_name>

6. Logs
   View commit history:
   git log

   View concise commit history:
   git log --oneline

   View last N commits:
   git log -n <number>

7. Remote Repositories
   Add a remote repository:
   git remote add origin <repo_url>

   View remote repositories:
   git remote -v

   Remove a remote repository:
   git remote remove <remote_name>

8. Pushing & Pulling
   Push changes to a remote repository:
   git push origin <branch_name>

   Push all branches to remote:
   git push --all origin

   Pull changes from a remote repository:
   git pull origin <branch_name>

   Fetch changes from a remote repository:
   git fetch origin

9. Undoing Changes
   Unstage a file (remove from index but keep in working directory):
   git rm --cached <filename>

   Undo last commit (keep changes):
   git reset --soft HEAD~1

   Undo last commit (remove changes completely):
   git reset --hard HEAD~1

   Revert a commit:
   git revert <commit_id>

10. Stashing Changes
    Save uncommitted changes temporarily:
    git stash

    List all stashes:
    git stash list

    Apply the most recent stash:
    git stash apply

    Apply a specific stash:
    git stash apply stash@{n}

    Remove a specific stash:
    git stash drop stash@{n}

    Remove all stashes:
    git stash clear

11. Tags
    Create an annotated tag:
    git tag -a v1.0 -m "Version 1.0"

    Create a lightweight tag:
    git tag v1.0

    List all tags:
    git tag

    Push a tag to remote:
    git push origin <tag_name>

    Delete a tag:
    git tag -d <tag_name>

12. Git Ignore
    Create a `.gitignore` file:
    touch .gitignore

    Edit `.gitignore` file:
    nano .gitignore

    Add patterns to ignore:
    (inside `.gitignore` file)
    *.log
    node_modules/
    .env

13. Git Cleanup
    Remove untracked files and directories:
    git clean -fd

14. Miscellaneous
    View all files, including hidden ones:
    ls -a

    Clear terminal screen:
    clear

    View command history:
    history
