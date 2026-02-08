# ⚔️ Merge Conflicts – When Git Gets Confused

Welcome to the **Merge Conflicts** module! Conflicts happen when two people change the same line of a file at the same time. Don't panic—Git just needs your help to decide which version to keep.

## 🎯 What You'll Learn

- **Understanding** why conflicts occur
- **Identifying** conflict markers
- **Resolving** conflicts manually
- **Completing** the merge

---

## 🛠️ Key Concepts

### 1. What Does a Conflict Look Like?
When you try to merge and Git can't automatically figure it out, it modifies your file to show both versions:

```markdown
<<<<<<< HEAD
This is my change on the main branch.
=======
This is the incoming change from the feature branch.
>>>>>>> feature-branch
```

- **`<<<<HEAD`**: Your current changes.
- **`=======`**: The separator.
- **`>>>>branch`**: The incoming changes.

### 2. How to Resolve?

1. Open the file in your code editor.
2. Decide which code to keep (or keep both).
3. Delete the conflict markers (`<<<<`, `====`, `>>>>`).
4. **Save** the file.
5. **Add** the resolved file:
   ```bash
   git add file.txt
   ```
6. **Commit** the merge:
   ```bash
   git commit -m "Resolved merge conflict"
   ```

---

## 📝 Activity

1. Create a file `conflict.txt` on `main` with "Line 1: Hello".
2. Create and switch to a branch `test-conflict`.
3. Change "Line 1" to "Line 1: Hi" and commit.
4. Switch back to `main`.
5. Change "Line 1" to "Line 1: Hey" and commit.
6. Try to merge: `git merge test-conflict`. Boom! Conflict. 💥
7. Fix it manually and commit!

Happy Coding! 🚀
