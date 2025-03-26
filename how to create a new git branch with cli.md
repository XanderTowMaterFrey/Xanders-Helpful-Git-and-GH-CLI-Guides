# **How To Create A New Branch Using Gh And Git CLI**

Hello, I am Xander and I will be showing you how to create a new branch using the gh and git CLI.

This is useful for general practice and for those who are new to the CLI version of git. I hope you find this helpful!

This will help you learn how to use your IDE for a more effective workflow with the developer's mythical laptop and GitHub.

## Steps

---

### Step 0 :: PrepWork

##### **---This can be skipped if you have a token setup \ alternate login method in place---**

<!-- Optional Step If Youre Set Up Right -->

```sh
gh auth login
```

### Step 1 :: Create A New Repo

#### **Save the output of the following command, it will be used later**

```sh
gh repo create my-new-repo --private
```

<!--dont forget to save that link!!! All it needs is .git at the end-->

---

### Step 2a :: Prepare Your Local Environment

````sh

#### **Prepare your local environment**

```sh
cd path/to/your/project
git init
````

---

### Step 2b :: Prepare The New Branch

#### **Add all files to the main branch and get ready for takeoff!!!**

```sh
git add -A
git commit -m "purpose of repo"
```

---

### Step 3 :: Create The New Branch

#### **Create the branch you will be using**

```sh
git checkout -b name-of-branch
```

---

### Step 4 :: Add Files To The New Branch And Push Them To Github!!

#### **And takeoff!!! This is the final step!**

```sh
git remote add origin https://github.com/your-username/my-new-repo.git
git push -u origin name-of-branch
```

---

Congratulations, [^1] you have created a new branch and pushed it to your repo!!!

---

[^1]: Thank you for taking the time to read my guide on creating a git repo with CLI!
