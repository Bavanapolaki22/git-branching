## Level 1: Introduction to Git Commits
This level introduces the basic concept of a Git commit.
Each commit represents a snapshot of the project at a specific point in time.
The goal is to understand how commits are created sequentially on the `main` branch.

<img width="1919" height="938" alt="Screenshot 2025-12-23 110628" src="https://github.com/user-attachments/assets/a3a13ac4-f900-4ae3-94ed-afd8cd594cc6" />


## Commands Used

```bash
git commit
git commit
```

## Level 2: Branching in Git


This level introduces **branches** in Git.
A branch allows you to work on a feature or fix independently without affecting the main codebase.

<img width="1914" height="951" alt="Screenshot 2025-12-23 110907" src="https://github.com/user-attachments/assets/d606848f-698b-4e3a-b22d-d1e8e03f0521" />


## Commands Used

```bash
git branch bugFix
git checkout bugFix
```

---

## Level 3: Merging in Git

This level demonstrates how to **merge one branch into another**.
Changes made in `bugFix` are merged back into `main`.

<img width="1919" height="945" alt="Screenshot 2025-12-23 111628" src="https://github.com/user-attachments/assets/784b465c-e132-4b98-b885-ca717b453c53" />


## Commands Used

```bash
git branch bugFix
git checkout bugFix
git commit
git checkout main
git commit
git merge bugFix
```

---

## Level 4: Rebase Introduction


This level introduces **rebasing**, an alternative to merging.
Rebase rewrites commit history by placing one branch’s commits on top of another branch.

<img width="1919" height="937" alt="Screenshot 2025-12-23 111845" src="https://github.com/user-attachments/assets/0de8f820-a465-437a-83d3-d3bd184e6019" />


## Commands Used

```bash
git branch bugFix
git checkout bugFix
git commit
git checkout main
git commit
git checkout bugFix
git rebase main
```




## Level 5: Detach Yo’ HEAD
This level explains the concept of a **detached HEAD** state.
Normally, `HEAD` points to a branch. In detached HEAD mode, `HEAD` points **directly to a commit**, not a branch.

<img width="1919" height="943" alt="1" src="https://github.com/user-attachments/assets/5bd166e1-b821-4a27-947a-ee5607ca8cc8" />

## Commands Used

```bash
git checkout c4
```

---

## Level 6: Relative Refs ( ^ )
This level introduces **relative references** using the caret (`^`) operator.
The caret allows navigation to a commit’s **parent**.

<img width="1912" height="953" alt="2" src="https://github.com/user-attachments/assets/a78ccbe6-a55b-45cf-a970-a0c7c1d906b3" />

### Commands Used

```bash
git checkout c3
```

##  Level 7: Relative Refs #2 ( ~ )
This level extends relative references using the tilde (`~`) operator and **force-moving branches**.

<img width="1915" height="938" alt="3" src="https://github.com/user-attachments/assets/677fd71a-e994-4878-a812-d99528f3316b" />


###  Commands Used

```bash
git checkout HEAD~1
git branch -f main C6
git branch -f bugFix C0
```


##  Level 8: Reversing Changes in Git
This level explains how to **undo changes** using `reset` and `revert`, and the difference between **local** and **pushed** commits.

<img width="1919" height="892" alt="4" src="https://github.com/user-attachments/assets/7ef13bdd-952d-4289-ac5b-fbd70422c2da" />


###  Commands Used

```bash
git checkout local
git reset c1

git checkout main
git commit

git checkout pushed
git revert HEAD
```




##  Level 9: Cherry-pick (Introduction)
This level introduces **`git cherry-pick`**, which allows you to **apply specific commits** from other branches into the current branch without merging the entire branch.

Instead of merging all changes, you can pick **only the required commits** by referencing their commit IDs.

<img width="1919" height="879" alt="5" src="https://github.com/user-attachments/assets/38be62fd-1d20-449d-a3ee-e99e6d6b11ae" />


###  Commands Used

```bash
git cherry-pick c3 c4 c7
```


##  Level 10: Interactive Rebase (Introduction)
This level introduces **interactive rebase**, which allows you to **edit, reorder, squash, or drop commits** before applying them on a new base.

Interactive rebase gives full control over commit history.

<img width="1919" height="878" alt="6" src="https://github.com/user-attachments/assets/16aa5eaf-c46d-489d-b8e7-25c078965b54" />


###  Commands Used

```bash
git rebase -i HEAD~4
```

