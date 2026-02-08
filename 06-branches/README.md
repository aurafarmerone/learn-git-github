# 🌿 Git Branches – Parallel Universes for Your Code

Welcome to the **Git Branches** module! Learn how to work on different features or fixes simultaneously without messing up your main project.

## 🎯 What You'll Learn

- **Creating** branches
- **Switching** between branches
- **Merging** changes back to the main branch
- **Deleting** branches

---

## 🛠️ Key Commands

### 1. `git branch <name>`
Creates a new branch. It does not switch to it automatically.

```bash
git branch feature-login
```

### 2. `git checkout <name>` OR `git switch <name>`
Switches to the specified branch. `git switch` is the newer, recommended command.

```bash
git switch feature-login
```

- Create and switch in one go:
  ```bash
  git checkout -b feature-login
  # OR
  git switch -c feature-login
  ```

### 3. `git merge <branch>`
Combines the history of the specified branch into the current branch. Usually, you switch to `main` first and then merge the feature branch into it.

```bash
git switch main
git merge feature-login
```

### 4. `git branch -d <name>`
Deletes a branch once it has been merged.

```bash
git branch -d feature-login
```

---

## 📝 Activity

1. Create a new branch called `dev`.
2. Switch to `dev`.
3. Create a file `dev.txt` and commit it.
4. Switch back to `main`. Note that `dev.txt` disappears!
5. Merge `dev` into `main` to bring your changes back.

Happy Coding! 🚀
