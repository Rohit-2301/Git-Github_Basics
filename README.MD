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
