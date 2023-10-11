# Github Repository Setup

## 1. Create Repository

### 1.1 From Github Website

  a. From Github Dashboard, click New Repository button.

  ---
  ![Click New Repository](/assets/repository-dashboard.png)
  
  ---

  b. Enter the repository name, repository description, repository status ( public / private ) and add readme.md automatically by checking (if needed)

  ---
  ![Fill New Repository Form](/assets/repository-detail.png)

  ---
  c. Your Repository is ready !!

  ---
  ![Repository is Ready](/assets/repository-ready.png)

  ---

## 2. Clone Repository to Local

  a. Open your repository on **Github**.

  ---
  ![Repository Url](/assets/repository-url.png)

  ---

  b. Copy the Repository URL.

  c. Run ``git clone`` on your **Terminal**.

  ```
  git clone https://github.com/<username>/<repository>.git .
  ```

  **Example :**

  ```
  git clone https://github.com/ku2h7/W0_Tutorial.git .
  ```

## 3. Push Directory or File into Github

  a. Create a file, ex. readme.md.

  ---
  ![Create New File on Local](/assets//repository-newfile.png)

  ---

  b. Add file with command line.

  ```
  git add <your_file_directory>
  ```

  **Example :**
  ```
  git add readme.md
  ```
---
  c. Commit your progress with command line.
  ```
  git commit -m 'Your Message'
  ```

  **Example :**
  ```
  git commit -m 'First Commit'
  ```
---
  d. Push your commit to the repository that has been created. Follow the following command line.
  ```
  git push origin <your_branch>
  ```

  **Example :**
  ```
  git push origin main
  ```

>**NOTE: Before adding file / directory, switch to the branch you want to push.**
---

## 4. Git Branch Instruction

### 4.1 Create New Branch

  You can create new branch with following command line:
  ```
  git checkout -b <your_branchname>
  ```

  **Example :**
  ```
  git checkout -b Kukuh.Module1
  ```

### 4.2 Show Current Branch

  To see your current branch on **Terminal**, follow this command line:

  ```
  git branch
  ```

  #### Result

  ---
  ![Branch List](/assets/branchlist.png)

  ---

### 4.3 Move to Another Branch

  For move to another branch, use the following command line:
  ```
  git checkout <your_destination_branch>
  ```

  **Example :**
  ```
  git checkout develop
  ```

### 4.4 Remove Branch

On **Github**, there are 2 types of branches, namely **Local Branch** and **Remote Branch**.
The local branch is the branch that is in your local, while the remote branch is the branch that you have pushed to **Github**.

#### 4.4.1 Remove Local Branch

To remove Local Branch, use the following command line:
```
git branch -D <branchname>
```

**Example :**
```
git branch -D kenangan_mantan
```

> **NOTE :** before delete Local Branch, you need to move to another branch. Besides using **-D**, you can also use **--delete**.

#### 4.4.2 Remove Remote Branch

To remove Remote Branch, use the following command line:
```
git push origin --delete <branchname>
```

**Example :**
```
git push origin --delete masa_lalu
```
