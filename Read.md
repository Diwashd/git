## **Git commands**

---

### **Git Basic Commands**

1. **`git init`**  
   Initializes a new Git repository in the current directory.

2. **`git clone <repository-url>`**  
   Creates a local copy of a remote repository.

3. **`git status`**  
   Displays the current state of the working directory and staging area.

4. **`git add <file>`**  
   Adds changes from the specified file to the staging area.

5. **`git commit -m "<message>"`**  
   Records changes in the repository with a descriptive message.

6. **`git log`**  
   Shows the commit history of the current branch.

7. **`git diff`**  
   Displays changes between the working directory and the staging area.

8. **`git branch`**  
   Lists, creates, or deletes branches.

9. **`git branch <branch-name>`**  
   Creates a new branch.

10. **`git branch -d <branch-name>`**  
    Deletes the specified branch (fails if the branch hasn't been merged).

11. **`git checkout <branch-name>`**  
    Switches to the specified branch.

12. **`git checkout -b <branch-name>`**  
    Creates and switches to a new branch.

13. **`git merge <branch-name>`**  
    Merges the specified branch into the current branch.

14. **`git reset <file>`**  
    Removes a file from the staging area, keeping the changes in the working directory.

15. **`git reset --hard`**  
    Resets the working directory and staging area to the last commit, discarding all local changes.

16. **`git revert <commit>`**  
    Creates a new commit that undoes the changes from the specified commit.

17. **`git rm <file>`**  
    Removes a file from the working directory and staging area.

18. **`git stash`**  
    Stashes changes that are not yet committed, saving them temporarily.

19. **`git stash pop`**  
    Applies the most recent stash and removes it from the stash list.

---

### **Working with Remotes**

1. **`git remote -v`**  
   Lists all remotes associated with the current repository, along with their URLs.

2. **`git remote add <name> <url>`**  
   Adds a new remote repository with the specified name and URL.

3. **`git fetch <remote>`**  
   Downloads new commits from the remote repository but does not merge them.

4. **`git pull <remote> <branch>`**  
   Fetches and merges changes from the specified remote branch into the current branch.

5. **`git push <remote> <branch>`**  
   Pushes local commits to the specified remote branch.

6. **`git push --force`**  
   Forces pushing changes to a remote, even if it would overwrite remote changes.

7. **`git push --set-upstream <remote> <branch>`**  
   Sets the upstream tracking for the branch to the specified remote.

8. **`git remote rm <name>`**  
   Removes the specified remote from the repository.

---

### **Branching and Merging**

1. **`git merge <branch>`**  
   Merges changes from the specified branch into the current branch.

2. **`git rebase <branch>`**  
   Re-applies commits from the current branch on top of the specified branch, rewriting history.

3. **`git cherry-pick <commit>`**  
   Applies the changes from a specific commit onto the current branch.

4. **`git branch -a`**  
   Lists all local and remote branches.

5. **`git branch -r`**  
   Lists only the remote branches.

6. **`git merge --no-ff`**  
   Creates a merge commit even if the merge could be fast-forwarded.

7. **`git merge --squash <branch>`**  
   Combines all changes from the specified branch into a single commit.

---

### **Working with Tags**

1. **`git tag`**  
   Lists all tags in the repository.

2. **`git tag <tag-name>`**  
   Creates a new tag at the current commit.

3. **`git tag -a <tag-name> -m "<message>"`**  
   Creates an annotated tag with a message.

4. **`git push <remote> <tag>`**  
   Pushes a tag to the remote repository.

5. **`git push --tags`**  
   Pushes all tags to the remote repository.

6. **`git tag -d <tag-name>`**  
   Deletes a local tag.

---

### **Undoing Changes**

1. **`git checkout -- <file>`**  
   Discards changes in the working directory for the specified file.

2. **`git reset <commit>`**  
   Resets the current branch to the specified commit, but leaves working directory changes intact.

3. **`git reset --soft <commit>`**  
   Resets the HEAD pointer to the specified commit and leaves changes staged.

4. **`git reset --hard <commit>`**  
   Resets the HEAD pointer, staging area, and working directory to the specified commit, discarding all changes.

---

### **Advanced Commands**

1. **`git reflog`**  
   Displays the history of changes to the repository’s HEAD, useful for recovering lost commits.

2. **`git ls-files`**  
   Lists all tracked files in the repository.

3. **`git config`**  
   Configures Git settings such as user name, email, etc.

4. **`git config --global <key> <value>`**  
   Sets a global configuration value (e.g., user name or email).

5. **`git blame <file>`**  
   Shows line-by-line commits and authorship for a file.

6. **`git log --oneline`**  
   Shows a compact version of the commit history, one commit per line.

7. **`git log --graph`**  
   Displays a visual representation of the commit history as a graph.

8. **`git log --author="<author-name>"`**  
   Filters commits by author.

---

### **Flagged Options**

1. **`-v`**: Used with `git remote` (e.g., `git remote -v`), it stands for **verbose** and shows additional information.
2. **`-d`**: Used with `git branch` (e.g., `git branch -d`), it stands for **delete** and removes a branch.
3. **`--hard`**: Used with `git reset` (e.g., `git reset --hard`), it discards all local changes.
4. **`--no-edit`**: Used with `git pull` to avoid editing the merge commit message automatically.
5. **`--force`**: Used with `git push` (e.g., `git push --force`), it forces the push, even if it will overwrite remote changes.
6. **`--squash`**: Used with `git merge` (e.g., `git merge --squash`), it combines all commits into a single commit.

---

This is a comprehensive list of **Git commands** with brief explanations and flags where applicable. Let me know if you need more details on any of them or would like further examples!
