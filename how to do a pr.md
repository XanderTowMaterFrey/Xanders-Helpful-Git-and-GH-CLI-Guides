# **How To Create A New Branch On Git Via CLI For A New PR**

Hello, I am Xander and I will be showing you how to create a new branch using the Git CLI for a new PR.

This is useful for general practice and for those who are new to the CLI version of Git. I hope you find this helpful!

This will help you learn how to use your IDE for a more effective workflow with the developer's mythical laptop and GitHub.

## Steps

---

### Step 0 :: Prep Work

#### **Ensure Everything Is Up To Date**

##### **---You May Need To Checkout Main / Origin / Master Or A Different Branch. It Will Be The Master Branch For The Repo You Are Working On---**

```sh
git checkout master
git pull
git status
```

---

### Step 1 :: New PR Branch Creation

#### **Create The Branch You Will Use In The PR**

```sh
git checkout -b branchForNewPR
```

---

### Step 2 :: Set Up The Branch With The Features You Want Via The Files You Want

#### **Add Desired Files You Want To Ensure Are Added To The PR**

##### **---Ensure That Everything Is Correct Via Git Status---**

##### **---TargetBranch Is The Branch You Work On With The Files You Would Like To Add To A PR. For Instance, If You Have A Main Branch And A Test Branch, You Would Merge The Features From The Test Branch Into The Main Branch Via A NewPRBranch. In This Example, The TargetBranch Would Be The Test Branch---**

```sh
git checkout TargetBranch -- filepath/file1 filepath/file2
git status
```

---

### Step 3 :: Ensure Everything Is Right As We Prepare To Push Everything

#### **Commit The Files And Features You Want To Add To The PR**

##### **---Ensure That Everything Is Correct Via Git Status And Diff (Develop / Origin / Master / Main Branch)---**

```sh
git add filepath1 filepath2
git commit -m "Adds files and features"
git status
git diff develop
```

#### **That's It, Everything Is Ready To Be Pushed To The New Branch As We Prepare To Create The PR!!!**

```sh
git push origin branchForNewPR
```

---

### Step 4 :: Create The PR

#### **Create The PR**

```sh
gh pr create --base master --head branchForNewPR --title "Add feature X" --body 'This PR adds feature X via updates [Y,Z, ETC...]'
```

---

Congratulations, [^1] you have created a new branch for your PR and pushed it to your repo!!!

---

[^1]: Thank you for taking the time to read my guide.
