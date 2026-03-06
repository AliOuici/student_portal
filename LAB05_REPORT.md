# LAB05 Report

## 1. What does HEAD represent?

`HEAD` in Git is a pointer to the **current commit you are working on**.  
- Usually, it points to the latest commit of the branch you have checked out.  
- When you switch branches, `HEAD` moves to the tip of the new branch.  
- Essentially, it represents the **current state of your working directory** in the repository.

---

## 2. Under what conditions does a merge conflict occur?

A merge conflict occurs when Git cannot automatically combine changes from two branches.  
This usually happens when:  
- The same line of a file has been modified differently in two branches, or  
- One branch deletes a file that the other branch modifies.  

Git will mark the conflicting sections in the file, and you need to **manually resolve** the conflict before committing.

---

## 3. What is the difference between `git clone` and `git pull`?

- `git clone`  
  - Used to **create a copy of an entire remote repository** locally for the first time.  
  - Downloads all commits, branches, and files.  

- `git pull`  
  - Used to **update an existing local repository** with the latest changes from the remote.  
  - Essentially combines `git fetch` (download changes) and `git merge` (merge into the current branch).  
