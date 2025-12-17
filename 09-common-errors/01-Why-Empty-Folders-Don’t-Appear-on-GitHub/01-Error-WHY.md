# ❌ Why Empty Folders Don’t Appear on GitHub

This is a **very common Git mistake**, especially for beginners.

# Scenario

Taking a scenario inwhich you decided to create empty folders locally like this : 

You run commands like:

```bash
mkdir my-folder
git add .
git commit -m "Add folders"
git push
```
but after pushing to GitHub,You got surprised to see that the empty folders that you pushed recently are **missing** 😕 on GitHub


Why this happen ?

```text
my-folder/   ❌ not visible
```


Let’s understand **why this happens** and **how to fix it properly**.