# What Git exactly do? 🤓

**Git** is a version control system.

It helps you to :
1. Track changes in your files,
2. Go back in time if sth breaks,
3. Work in parallel with other people,
4. Keep history of what you have done.

---

# Git Commands 

### git init 🗂️

``` git
git init
```
- The first command when you want to using your Git.
it initializes a new git repository inside your folder.

***Hey git, follow me !*** 😁

when you command `git init`, git create a hidden folder called `.git` inside of your project directory. This folder contain everything that git need :

 ```
 git init = 
 Hey Git, Please start watching this folder and be ready to track my files and projects.
 ```

---

## Git Area 💻

We have 3 main area in Git :

1. Working Directory: where your actual code are. (What you edit)

2. Staging Area: Where to put your changes you want to save. (A waiting room)

3. Repository: The permanent history of your projects inside git. (Commit History)

---

## What is Stage ? 📥

Staging means you selecting which changes go to next snapshot.  The Main command is : 

```git
git add FileName
```

Or for add everything 

```git
git add .
```

Or for add files with similar name

```git 
git add "Pro*"
```
add all files that they have  ***Pro***  on their names.

---
## What is Commit ? 🖇️

Commiting means saving a snapshop of everything that's stage. After commiting, the snapshop is saved in git repository history forever. The command is :

```git 
git commit -m "Your Message"
```
---

## Git Status 📌

```git
git status
```
It shows your current state of your working directory and stage area. It shows us :

1. Which files tracked by git,
2. Which files have been changed but not staged,
3. Which files are staged and ready to commit,
4. Are there any untracked file ?

---

## Git Log 📑

```git
git log
```

A report of what git have done.
1. **Commit a3cd...** = Each commit has unique ID.
2. **Author** = Who made the commit ?
3. **Date** = When it was made ?
4. **Message** = What sb wrote in -m "X" during commiting.

---

## Git Diff ➖➕

```git 
git diff
```
What you changed but haven't staged yet.
It shows you the exact changes ***inside the files***. It tells you what's different between :

1. Working Directory Vs. Staging Area
2. Staging area Vs. Last commit 
   - In this case you may see two elements (-)/(+).

   ```diff
   - It means some lines have been removed.
   
   + It means some lines have been added.
   ```


```git
git diff --staged 
```
What has staged but not commited yet.
(Show me what changes happen in stage area)

```git 
git diff Head
```
compair working dir + staging with last commit.

---

## Git Reset 🔁
