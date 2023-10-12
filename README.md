# Github Repository Tutorial

## 1. Create Repository

a. From Github Dashboard, click New Repository button.

---
![Click New Repository](/assets/repository-dashboard.png)
---

b. Enter the repository name, repository description, repository status ( public / private ) and add readme.md automatically by checking (if needed)

---
![Fill New Repository Form](/assets/repository-detail.png)
---

Your Repository is ready !!

---
![Repository is Ready](/assets/repository-ready.png)
---

## 2. Initialize Repository

>**Note :** Before initialize your folder, reviously you created a repository in your `GitHub` account.

a. Open your specific directory on VS Code.

b. Create folder with this command line:

```
mkdir <your_folder_name>
```

**Example :**

```
mkdir my_assignment
```


c. Create a file, like readme.md.

d. Initialize New Repository in an exiting folder.

- For the first, initialize your exiting folder, with this command line:

> ```
> git init
> ```

- Add your file.

> ```
> git add readme.md
> ```

- Or add all file with following this command line:

> ```
> git add .
> ```

- Next, commit your change.

> ```
> git commit -m 'add README.md'
> ```

- Create branch for your commit.

> ```
> git branch -M <your_branch_name>
> ```

**Example :**

> ```
> git branch -M master
> ```

- Sync your local and Github Repository.

> ```
> git remote add origin https://github.com/<username>/<project_name>.git
> ```

**Example :**

> ```
> git remote add origin https://github.com/ku2h7/MyAssignment.git
> ```

- Push your changes, with this command line:

> ```
> git push -u origin <branch_name>
> ```

**Example :**

> ```
> git push -u origin master
> ```

## 3. Clone Repository to Local

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

## 4. Push Directory or File into Github

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

## 5. Git Branch Instruction

### 5.1 Create New Branch

You can create new branch with following command line:
```
git checkout -b <your_branchname>
```

**Example :**
```
git checkout -b Kukuh.Module1
```

### 5.2 Show Current Branch

To see your current branch on **Terminal**, follow this command line:

```
git branch
```

#### Result

---
![Branch List](/assets/branchlist.png)

---

### 5.3 Move to Another Branch

For move to another branch, use the following command line:
```
git checkout <your_destination_branch>
```

**Example :**
```
git checkout develop
```

### 5.4 Remove Branch

On **Github**, there are 2 types of branches, namely **Local Branch** and **Remote Branch**.
The local branch is the branch that is in your local, while the remote branch is the branch that you have pushed to **Github**.

#### 5.4.1 Remove Local Branch

To remove Local Branch, use the following command line:
```
git branch -D <branchname>
```

**Example :**
```
git branch -D kenangan_mantan
```

> **NOTE :** before delete Local Branch, you need to move to another branch. Besides using **-D**, you can also use **--delete**.

#### 5.4.2 Remove Remote Branch

To remove Remote Branch, use the following command line:
```
git push origin --delete <branchname>
```

**Example :**
```
git push origin --delete masa_lalu
```
