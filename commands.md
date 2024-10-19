# Git Command History

## 1. **Setting Up the Repository**
```bash
mkdir git-for-devops
cd git-for-devops/
git init
```
**Explanation**: 
1. Creates a directory (`git-for-devops`) and navigates into it.
2. Initializes a new Git repository in that directory.

## 2. **File Operations and Status Check**
```bash
vim hello-dosto.txt     # Create and edit a text file
git status              # Check the status of the repository
touch nibba.txt nibbi.txt
git add nibbi.txt
git status
git add nibba.txt
git status
```
**Explanation**:
1. Files are created (`hello-dosto.txt`, `nibba.txt`, `nibbi.txt`).
2. `git add` stages the files for committing.
3. Status checks show the changes in the working directory and staging area.

## 3. **Committing Changes**
```bash
git commit -m "initial commit"
git status
```
**Explanation**:
1. Commits the staged files with a message.
2. The status confirms no pending changes after the commit.

## 4. **Removing and Restoring Files**
```bash
git rm --cached nibba.txt   # Unstage nibba.txt without deleting the file
git restore nibbi.txt       # Restores the file from the latest commit
git status
```
**Explanation**:
1. Unstages the file `nibba.txt` but does not delete it.
2. Restores `nibbi.txt` back to its previous version.
3. Status checks the repository for updates.

## 5. **Setting Global Configurations**
```bash
git config --global user.name "AnirbanB13"
git config --global user.email "anirbanbanerjeeuv@gmail.com"
```
**Explanation**:
1. Sets the global user name and email for Git commits.

## 6. **Branching and Switching Branches**
```bash
git branch                    # List all branches
git checkout -b dev            # Create and switch to a new branch 'dev'
git checkout master            # Switch back to the master branch
git checkout dev               # Return to the 'dev' branch
```
**Explanation**:
1. Displays the current branches.
2. Creates a new branch called `dev` and switches to it.
3. Commands to switch between `master` and `dev` branches.

## 7. **Adding and Committing Changes in New Branch**
```bash
touch nibbu.txt
git add nibbu.txt
git commit -m "added nibbu"
```
**Explanation**:
1. A new file `nibbu.txt` is created and added to the staging area.
2. Changes are committed with a message.

## 8. **Viewing Commit History**
```bash
git log
git log --oneline           # Show concise commit history
```
**Explanation**:
1. Displays the full commit history of the repository.
2. Shows a simplified one-line-per-commit view.

## 9. **Other Git Operations**
```bash
git --help                  # Access Git help
git help -g                 # Get a list of available Git guides
clear                       # Clear the terminal
history                     # View command history
```
**Explanation**:
1. The `help` commands provide useful Git documentation.
2. `clear` cleans up the terminal for a better view.
3. `history` displays the command history in the terminal.
