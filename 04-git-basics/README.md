# 🌲 Git Basics – The Foundation

Welcome to the **Git Basics** module! Here, you'll learn the fundamental commands that you'll use 90% of the time when working with Git.

## 🎯 What You'll Learn

- **Initializing** a repository
- **Staging** files
- **Committing** changes
- Checking **status** and **history**

---

## 🛠️ Key Commands

### 1. `git init`
Initializes a new Git repository. This transforms a regular folder into a Git-tracked folder.

```bash
git init
```

### 2. `git add <file>`
Moves changes from the **Working Directory** to the **Staging Area**.

- Add a specific file:
  ```bash
  git add index.html
  ```
- Add **all** changed files in one go:
  ```bash
  git add .
  ```

### 3. `git commit -m "message"`
Saves your staged changes to the local repository history.

```bash
git commit -m "Initial commit"
```

> **Tip:** Always write clear and descriptive commit messages!

### 4. `git status`
Shows the state of your working directory and staging area. It tells you what's modified, staged, or untracked.

```bash
git status
```

### 5. `git log`
Displays the commit history.

```bash
git log
```

- For a more concise view:
  ```bash
  git log --oneline
  ```

---

## 📝 Activity

1. Create a new file named `hello.txt`.
2. Add some text to it.
3. Run `git status` to see it as untracked.
4. Run `git add hello.txt` to stage it.
5. Run `git commit -m "Add hello.txt"` to save it.
6. Run `git log` to see your commit!

Happy Coding! 🚀
