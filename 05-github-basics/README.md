# 🐙 GitHub Basics – Taking Your Code Online

Welcome to the **GitHub Basics** module! Learn how to share your code, collaborate with others, and work with remote repositories.

## 🎯 What You'll Learn

- **Creating** a remote repository on GitHub
- **Pushing** local code to GitHub
- **Cloning** existing projects
- **Pulling** updates

---

## 🛠️ Key Commands

### 1. `git remote add origin <url>`
Connects your local repository to a remote repository (like one on GitHub).

```bash
git remote add origin https://github.com/username/repo-name.git
```

### 2. `git clone <url>`
Downloads a project and its entire version history from a remote repository.

```bash
git clone https://github.com/username/project.git
```

### 3. `git push -u origin main`
Uploads your local commits to the remote repository. The `-u` flag sets the "upstream" tracking, so you can just type `git push` later.

```bash
git push -u origin main
```

### 4. `git pull`
Fetches and merges changes from the remote repository to your current local branch.

```bash
git pull origin main
```

---

## 📝 Activity

1. Create a new repository on GitHub (without a README).
2. Copy the HTTPS URL.
3. In your local terminal, navigate to your project folder.
4. Run:
   ```bash
   git remote add origin <your-url>
   git push -u origin main
   ```
5. Refresh your GitHub page to see your code online!

Happy Coding! 🚀
