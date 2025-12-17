# ❌ Why Empty Folders Don’t Appear on GitHub

This is a **very common Git mistake**, especially for beginners.

# Scenario

Taking a scenario inwhich you decided to create folders locally like this : 

You run commands like:

```bash
mkdir my-folder
git add .
git commit -m "Add folders"
git push
```
but after pushing to GitHub,You got surprised to see that the folders that you pushed recently are **missing** 😕 on GitHub


Why this happen ?

```text
my-folder/   ❌ not visible
```


Let’s understand **why this happens** and **how to fix it properly**.


## 🧠 The Reason (Important Concept)

> **Git does NOT track folders.**

Git only tracks **files and their content**.

So:
- A folder **with files** → ✅ tracked
- An **empty folder** → ❌ ignored

This is expected Git behavior.



## ✅ The Correct Solution: `.gitkeep`

### What is `.gitkeep`?

- A **convention**, not a Git feature
- An empty file used to keep directories in Git
- Widely used in open-source projects



### 🛠️ Step-by-Step Fix

#### 1️⃣ Create a `.gitkeep` file inside the empty folder

```bash
touch my-folder/.gitkeep
```

#### 2️⃣ Add, commit, and push

```bash
git add .
git commit -m "Keep empty folder using .gitkeep"
git push
```

✔️ The folder will now appear on GitHub



## ⭐ Best Practice (Recommended)

For learning or documentation repositories:

```text
09-error-empty-folders/
├── README.md
```

For future-use folders:

```text
src/
└── .gitkeep
```



## 🧪 Common Beginner Mistake

❌ Expecting Git to track folders automatically  
✅ Remember: **Git tracks files, not directories**



## 🎯 Interview Question

**Q: Why doesn’t Git track empty directories?**  
**A:** Because Git is a content-tracking system, not a filesystem tracker.



Happy learning 🚀  
This error alone teaches one of the most important Git fundamentals.

