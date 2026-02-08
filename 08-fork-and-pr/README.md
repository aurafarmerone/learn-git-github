# 🍴 Fork & Pull Request – Contributing to Open Source

Welcome to the **Fork & PR** module! This is the heart of open source collaboration. You'll learn how to contribute to projects you don't own.

## 🎯 What You'll Learn

- **Forking** a repository
- **Creating a Pull Request (PR)**
- **Syncing** your fork with the original repository

---

## 🛠️ Key Concepts

### 1. What is a Fork?
A **fork** is a copy of a repository that you manage. Forking allows you to experiment with changes without affecting the original project.

### 2. The Workflow

1.  **Fork** the project on GitHub.
2.  **Clone** your fork locally.
    ```bash
    git clone https://github.com/your-username/project.git
    ```
3.  **Create a branch** for your changes.
    ```bash
    git switch -c fix-typo
    ```
4.  **Make changes** and **commit**.
5.  **Push** to your fork.
    ```bash
    git push origin fix-typo
    ```
6.  **Open a Pull Request** on the original repository on GitHub to propose your changes.

### 3. Syncing a Fork
To keep your fork up-to-date with the original repository (often called `upstream`):

1.  Add the upstream remote:
    ```bash
    git remote add upstream https://github.com/original-owner/project.git
    ```
2.  Fetch and merge upstream changes:
    ```bash
    git fetch upstream
    git merge upstream/main
    ```

---

## 📝 Activity

1. Find a repository you want to contribute to (or a practice one).
2. Click the **Fork** button.
3. Clone your fork.
4. Make a small change (like fixing a typo).
5. Push it and open a PR!

Happy Coding! 🚀
