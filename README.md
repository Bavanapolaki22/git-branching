Level 1: Introduction to Git Commits
This level introduces the basic concept of a Git commit.
Each commit represents a snapshot of the project at a specific point in time.
The goal is to understand how commits are created sequentially on the `main` branch.

<img width="1919" height="938" alt="Screenshot 2025-12-23 110628" src="https://github.com/user-attachments/assets/a3a13ac4-f900-4ae3-94ed-afd8cd594cc6" />


Commands Used

```bash
git commit
git commit
```

 Level 2: Branching in Git


This level introduces **branches** in Git.
A branch allows you to work on a feature or fix independently without affecting the main codebase.

<img width="1914" height="951" alt="Screenshot 2025-12-23 110907" src="https://github.com/user-attachments/assets/d606848f-698b-4e3a-b22d-d1e8e03f0521" />


Commands Used

```bash
git branch bugFix
git checkout bugFix
```

---

 Level 3: Merging in Git

This level demonstrates how to **merge one branch into another**.
Changes made in `bugFix` are merged back into `main`.

<img width="1919" height="945" alt="Screenshot 2025-12-23 111628" src="https://github.com/user-attachments/assets/784b465c-e132-4b98-b885-ca717b453c53" />


Commands Used

```bash
git branch bugFix
git checkout bugFix
git commit
git checkout main
git commit
git merge bugFix
```

---

Level 4: Rebase Introduction


This level introduces **rebasing**, an alternative to merging.
Rebase rewrites commit history by placing one branch’s commits on top of another branch.

<img width="1919" height="937" alt="Screenshot 2025-12-23 111845" src="https://github.com/user-attachments/assets/0de8f820-a465-437a-83d3-d3bd184e6019" />


Commands Used

```bash
git branch bugFix
git checkout bugFix
git commit
git checkout main
git commit
git checkout bugFix
git rebase main
```
