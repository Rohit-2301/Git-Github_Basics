# 🚀 Git & GitHub Basics  

Git is a **version control system** that helps developers manage and track changes in their code, while GitHub is a **cloud-based platform** for hosting Git repositories and collaborating with others. This guide covers the essential Git commands and workflows to get you started.

---

## 📌 What is Git?  

Git is a **distributed version control system** that allows multiple developers to work on a project efficiently, keeping track of changes and enabling easy collaboration.

### 🔧 Basic Git Commands and Their Usage  

| Command | Description |
|---------|-------------|
| `git init` | Initializes a new Git repository in your local project directory. |
| `git clone <repo_url>` | Downloads (clones) a repository from GitHub to your local machine. |
| `git status` | Shows the current state of your repository (modified, staged, or untracked files). |
| `git add <file>` | Adds a specific file to the staging area before committing. |
| `git add .` | Stages all modified and new files in the repository. |
| `git commit -m "message"` | Saves (commits) the staged changes with a meaningful message. |
| `git push origin <branch>` | Uploads (pushes) local commits to a remote GitHub repository on the specified branch. |
| `git pull origin <branch>` | Fetches and merges the latest changes from a remote repository into your local branch. |
| `git log` | Displays a history of commits made in the repository. |
| `git branch` | Lists all branches in the repository and highlights the current branch. |
| `git checkout -b <new-branch>` | Creates and switches to a new branch for feature development. |
| `git merge <branch>` | Merges changes from another branch into the current branch. |
| `git reset --hard HEAD~1` | Removes the last commit permanently from history. |
| `git revert <commit_id>` | Creates a new commit that undoes a previous commit without modifying history. |
| `git checkout -- <file>` | Discards changes made to a specific file before committing. |
| `git remote -v` | Displays the URLs of remote repositories linked to your project. |
| `git stash` | Temporarily saves changes that are not yet committed, allowing you to switch branches. |
| `git stash pop` | Restores the most recently stashed changes. |
| `git rm <file>` | Removes a file from the repository and deletes it from the working directory. |

---

## 📌 What is GitHub?  

GitHub is a **web-based platform** that hosts Git repositories, making it easy for developers to collaborate on projects, track issues, and review code.

### 🔗 Basic GitHub Workflow  

1. **Create a Repository**  
   - Go to [GitHub](https://github.com) → Click **New Repository** → Enter a name → Click **Create Repository**  

2. **Clone the Repository (Download it Locally)**  
   ```sh
   git clone <repo_url>
   cd <repo_name>
   ```

---

## 📌 Create a GitHub Repository Using Terminal

Follow these steps to create and push a new GitHub repo using terminal:

### ✅ Step 1: Create a New Directory and Initialize Git
```sh
mkdir <project_name>
cd <project_name>
git init
```

### ✅ Step 2: Create Files and Make Initial Commit
```sh
echo "# Project Title" > README.md
git add .
git commit -m "Initial commit"
```

### ✅ Step 3: Create a Repository on GitHub
- Go to [GitHub](https://github.com) → New Repository → Enter name → Click **Create Repository**
- DO NOT initialize with README, .gitignore, or license.

### ✅ Step 4: Link Local Repo to GitHub Remote and Push
```sh
git remote add origin https://github.com/<your_username>/<repo_name>.git
git branch -M main
git push -u origin main
```

---

## 📌 Steps to Add a File to GitHub Using Git & VS Code  

Follow these steps to add and upload a new file to your GitHub repository:

### ✅ Step 1: Open Your Project in VS Code  
- Open **VS Code** and navigate to your project folder.

### ✅ Step 2: Create or Add a File  
- Add a new file or modify an existing file in the project directory.

### ✅ Step 3: Open Terminal in VS Code  
- Open the **terminal** (`Ctrl + ~` on Windows/Linux or `Cmd + ~` on Mac).

### ✅ Step 4: Check the Status of Your Repository  
```sh
git status
```
- This shows any new, modified, or deleted files.

### ✅ Step 5: Add the File to Staging Area  
```sh
git add <filename>  # Adds a specific file
git add .  # Adds all new and modified files
```

### ✅ Step 6: Commit the Changes  
```sh
git commit -m "Added <filename>"
```
- Write a meaningful commit message describing the change.

### ✅ Step 7: Push the Changes to GitHub  
```sh
git push origin main
```
- If you're working on a different branch, replace `main` with your branch name.

### ✅ Step 8: Verify on GitHub  
- Go to your **GitHub repository** and check if the file is uploaded.

---

🚀 **Now your file is successfully added to GitHub!** 🎉

---

## 📌 Steps to Remove a File from GitHub Using Git & VS Code  

Follow these steps to remove a file from your GitHub repository:

### ✅ Step 1: Open Your Project in VS Code  
- Open **VS Code** and navigate to your project folder.

### ✅ Step 2: Open Terminal in VS Code  
- Open the **terminal** (`Ctrl + ~` on Windows/Linux or `Cmd + ~` on Mac).

### ✅ Step 3: Remove the File  
```sh
git rm <filename>
```
- This removes the file from your local repository.

### ✅ Step 4: Check the Status of Your Repository  
```sh
git status
```
- Verify that the file is marked as deleted.

### ✅ Step 5: Commit the Changes  
```sh
git commit -m "Removed <filename>"
```
- Write a meaningful commit message describing the removal.

### ✅ Step 6: Push the Changes to GitHub  
```sh
git push origin main
```
- If you're working on a different branch, replace `main` with your branch name.

### ✅ Step 7: Verify on GitHub  
- Go to your **GitHub repository** and check if the file is removed.

---

🚀 **Now your file is successfully removed from GitHub!** 🚗️
