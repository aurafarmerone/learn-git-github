# 03. Git Setup on Windows ⚙️

This guide explains **how to set up Git after installation**, including:

1. Verifying that Git is installed
2. Configuring your Git username and email
3. Removing old Git credentials
4. Logging in with a new account

This guide is beginner-friendly and follows Windows + Git Bash.



## 🔹 Step 1: Verify Git Is Installed

Before configuring Git, make sure it is installed correctly.

1. Open **Git Bash**
2. Run the command:

```bash
git --version
```

✅ Expected output:
```
git version 2.xx.x
```

If you see a version number, Git is installed correctly.



## 🔹 Step 2: Configure Git Username and Email

### ❓ Why is this setup required?

Git needs to know **who you are** so it can attach your name and email to every commit you make.

- Every Git commit stores **author information**
- GitHub uses this email to link commits to your profile
- Without this setup, Git may throw errors or show *unknown author*

✅ **Good news:** You only need to configure this **one time** on your system.
Git will remember it for all future projects.


### ✅ Set Global Username

```bash
git config --global user.name "Your Name"
```

Example:
```bash
git config --global user.name "Aura Farmer"
```

### ✅ Set Global Email

```bash
git config --global user.email "your@email.com"
```

Example:
```bash
git config --global user.email "aurafarmer@gmail.com"
```

### 🔍 Verify Configuration

```bash
git config --global --list
```

You should see:
```
user.name=Your Name
user.email=your@email.com
```



## 🔹 Step 3: Remove Old Git Credentials (Important)

### ❓ Why remove old credentials?

If you previously logged in with:
- The **wrong GitHub account**
- An **old email**
- Someone else’s credentials

Git will keep using them automatically and cause problems like:
- Pushing code to the wrong account
- Permission denied errors
- Commits not appearing on your GitHub profile

That’s why removing old credentials is necessary **only when switching accounts**.

On Windows, Git stores credentials using **Git Credential Manager**.

### ✅ Method 1: Remove Credentials Using Git (Recommended)

#### 🔸 Remove GitHub credentials

```bash
git credential-manager logout https://github.com
```

✔️ This safely removes saved login tokens.



### ✅ Method 2: Remove Credentials Manually (Windows Credential Manager)

Use this if Method 1 doesn’t work.

1. Press **Win + R**
2. Type:
   ```
   control
   ```
3. Open **Credential Manager**
4. Click **Windows Credentials**
5. Delete entries like:
   - `git:https://github.com`
   - `GitHub`

✔️ You are now fully logged out.



## 🔹 Step 4: Login with a New Account

After removing old credentials:

1. Go to any Git repository
2. Run:

```bash
git push
```

Git will now:
- Ask you to log in again
- Open a browser window
- Let you sign in with a **new GitHub account**

✔️ Login is now updated.


## 🎯 What’s Next?

Now your Git is fully set up ✅

You’re ready to:
- Create repositories
- Push code to GitHub
- Learn Git commands

➡️ Continue to **04-git-basics** 🚀


### 💡 Beginner Tip

> If Git asks for login again — that’s normal. It means credentials were cleared successfully 🙂

Happy Coding! ❤️

