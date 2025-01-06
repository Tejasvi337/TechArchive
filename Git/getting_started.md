# Git  

> **Git** is a distributed version control system (DVCS) that helps developers collaborate on projects, track changes, and manage code repositories efficiently. 

This guide will walk you through the essential steps to start using Git.

---

## **Content**  
- ### **Git Fundamentals**
- ### **Basic Git Commands**
- ### **Working with Remote Repositories**
- ### **Branching & Merging**
- ### **Undoing Changes & Fixing Mistakes**
- ### **Collaborating with Others**
- ### **Advanced Git Features**
- ### **Best Practices**

---

## **Topics**

### **Git Fundamentals**

- #### **How Git Stores Data**

- #### **Git FileTypes**

    - **.git**
    - **.gitignore**

---  

### **Git Basic Commands**

#### **1. Initializing Repositories**

- `git init`
- `git clone`
    - `git clone <url>`
    - `git clone <url> <new repo name>`

#### **2. Repository Status**

- `git status`
    - `git status --short`/`git status -s`
    - `git status <path>`

####  **3. Tracking and Staging Changes**

- `git add`
    - `git add .`
    - `git add -A`

#### **4. Commit Changes**

- `git commit`
    - `git commit -a`
    - `git commit -m "<message>"`
    - `git commit --amend`

#### **5. Viewing History**

- `git log`
    - `git log --oneline`
    - `git log -p`
    - `git log --stat`

#### **6. Viewing Changes**

- `git diff`
    - `git diff --staged`
    - `git diff <commit1> <commit2>`

#### **7. Removing Files**

- `git rm`
    - `git rm <file>`
    - `git rm --cached <file>`

#### **8. Moving and Renaming Files**

- `git mv <old_filename> <new_filename>`

#### **9. Ignoring Files**

- `.gitignore`

#### **10. Add Remote Server**

- `git remote add <remote_serve_url>`

#### **11. Configuration**

- `git config`
    - `git config --global user.name "<name>"`
    - `git config --global user.email "<email>"`
    - `git config --list`

---

### **Git Branching**

#### **1. List All Branch**

- `git branch`
    - `git branch -r`: List all remote branches
    - `git branch -a`: List all local and remote branches

#### **2. Create Branch**

- `git switch -c  <branch_name>`

#### **3. Switch Branch**

- `git switch <branch_name>`

#### **4. Delete Branch**

- `git branch -d <branch_name>`
    - `git branch -D <branch_name>`: Force delete

#### **5. Merge Branch**

- `git merge <branch_name>`

---

### **Git Remote Repositories**

#### **1. Add Remote Repository**

- `git remote add <name> <url>`

#### **2. Remove Remote Repository**

- `git remote remove <name>`

#### **3. List Remote Repositories**

- `git remote -v`

#### **4. Fetch Changes**

- `git fetch <remote>`

#### **5. Pull Changes**

- `git pull <remote> <branch>`

#### **6. Push Changes**

- `git push <remote> <branch>`

---

### **Git Stash**

#### **1. Stash Changes**

- `git stash`

#### **2. List Stashes**

- `git stash list`

#### **3. Apply Stash**

- `git stash apply`

#### **4. Drop Stash**

- `git stash drop`

#### **5. Pop Stash**

- `git stash pop`
---

### **Best Practices**

#### **Commit Messages**

**Standard Format**
A commit message should follow this structure
```text
<type>: <short, imperative summary>

<optional detailed description>
<optional references/issues>
```
Example
```text
feat: add user authentication

Implemented user login and signup with JWT authentication. Includes password hashing and email verification.
Closes #42
```  
**Concise Summary**
- Keep the first line **50 characters or fewer**.
- Use the **imperative mood** (e.g., "Add feature" instead of "Added feature").
- Do **not** end with a period.

**Consistent Type**
Use a type prefix:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation update
- `style`: Formatting changes
- `refactor`: Code restructuring
- `test`: Adding/fixing tests
- `chore`: Maintenance tasks

**Context in the Body**
- Explain **what changed** and **why**.
- Keep lines **≤ 72 characters** for readability.



#### **Documentation**