# Git-and-Github

### ❤️ What is Git ?
➔ Free and openSource version control system ( vcs means tools that help to track changes in code ) <br/>
➔ VCS track history and it helps to collaborate <br/>

### ❤️ What is GitHub ?
➔ Website where we host repositories online <br/>
➔ we can also track our initiate , update , delete history. <br/>
➔ generally we create files/folders using mouse but we can create them using terminal. Likewise, we can directly upload on github but a good developer prefer to do changes using Terminal. <br/>

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### 💚 Using Git
➔ Git is already installed in macOs and Linux. But, in windows we are installing Git-Bash which already have git <br/>
➔ check that git installed or not `git --version` if any version available then git is installed <br/>
<br/>
➔ ways to use git
1) Command line -- popular way
2) IDE/code editors like VScode
3) Graphical user interface like GitKraken

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━<br/>
<br/>
⚠️**Note**- everywhere in codes if i am using <name> means you have to write proper thing at something expect < , > like ` " <name> " ` so the answer of this is ` "parth" ` <br/>
<br/>
<br/>
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━<br/>
### 💛 Configuring Git

✔️ `git config --global user.name "<userName>"` (write username at userName)<br/>
✔️ `git config --global user.email "<someone@gmail.com>" `(enter your email) <br/>
✔️ `git config --list` (to check that details are saved or not )<br/>

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ <br/>

### 💙 Git with VScode
➔ we can also open intergrated terminal with vscode (From the menu, use the Terminal > New Terminal or View > Terminal menu commands)<br/>
➔ same as terminal/git-bash <br/>

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ <br/>

### 💚 Basic commands

✔️ `git clone <link>` = clone = cloning a repository on our local machine <br/>
💤 *how to generate links - go to the repo on gitHub and there is button named CODE click there and copy HTTPS link*  <br/>
<br/>
✔️ `git status` = status = display the state of code <br/>
<br/>
<img src="https://support.nesi.org.nz/hc/article_attachments/360004194235/Git_Diagram.svg" width=600px height=300px>

✔️ `git add <fileName>` = adds new or changed files in working directory to the git staging area  <br/>
✔️ `git commit -m "some message"` = record the change <br/>
✔️ `git push origin main`  = upload local repo content to remote repo <br/>
<br/>
♻️ first clone the github repo on local machine , then check git status , if any file which created newly is untracked then do git add then if we do some changes in that file then again do git commit means save , then if we want to push/upload this file on github then do git push origin main <br/>

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/>

### 💜 Init command - used to create new git repo
➔ sometimes we started to create project from scratch in our local system and if we want to make new repo then <br/>
<br/>
✔️ `git init` =  <br/>
✔️ `git remote add origin <link>`  = we are adding the link of repo where we want to push our folders from local system <br/>
✔️ `git remote -v` = to verify remote <br/>
✔️ `git branch` = to check branch name <br/>
✔️ `git branch -M main` = to rename branch name to "main" <br/>
✔️ `git push origin main`  <br/>

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### 💚 Git branches
➔ it creates the duplicate of main/master branch to work on features or fix bugsv 

![](https://wac-cdn.atlassian.com/dam/jcr:86eba9ec-9391-45ea-800a-948cec1f2ed7/Branch-2.png)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### 💚 branch commands

✔️ `git branch` = to check branch <br/>
✔️ `git branch -M main` = to rename branch <br/>
✔️ `git checkout <branch-name> ` = to navigate <br/>
✔️ `git checkout -b <new-branch-name>` = to create new branch <br/>
✔️ `git branch -d <branch-name>` = to delete branch <br/>

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### 💛 Merging code
➔ merging branches <br/> 

✔️ `git diff <branch-name>` = to compare commits,branches,files <br/> 
✔️ `git merge <branch-name>` = to merge 2 branches <br/>  
OR create a PR(Pull Request) <br/> 
 <br/> 
 
💙 **Pull Request** <br/> 
➔ it lets you tell others about the changes you have pushed to a branch in a repo on github<br/>  ➔ we can get the button "Compare & pull request" of PR at the github repo for merging<br/> 

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### 🧡 Pull command

➔ Now the changes are already done on github using PR from github web and so there is not any changes on our local working system and so we have to do Pull command to see the same repo as github ( first push and then pull )  <br/>
✔️ `git pull origin main`

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### 💛 Merge conflicts
➔ like we have 2branches and at the same place there are different chnages available and so there is conflict <br/> 
➔ Vs code already have feature it will ask about it and then you have to select the changes or that is your wish what will be the change  <br/> 

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### 💚 Fixing Mistakes

1️⃣ Staged (git status) changes <br/> 
✔️ `git reset <fileName>` (for remove change the particular file)  <br/> 
✔️ `git reset` (for remove the change for all files)  <br/> 

2️⃣ commited changes(for one commit)  <br/> 
✔️ `git reset HEAD~1` (here head pointer is pointing last commit)  <br/> 

3️⃣ commited changes(for many commits)  <br/> 
✔️ `git reset <commit-hash>`  <br/> 
✔️ `git reset --herd <commit-hash>`  <br/> 

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### 💛 What is Forking ?
➔ a fork is newrepo that shares code and visibility settings with original "upstream" repo  <br/> 
➔ fork is rough copy  <br/> 
➔ usage- open source contribution  <br/> 
 
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### differance

```
git diff
```

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  <br/> 

### revert to previous version
![VvIxF](https://github.com/parthmern/Git-and-Github/assets/125397720/4a6b792e-aa3c-43de-b8de-80e1863d74b8)
![1_045T7UdsT40cRIwCAnUJ0w](https://github.com/parthmern/Git-and-Github/assets/125397720/0b00e071-523e-4e41-938d-624263bb0de4)

```
https://stackoverflow.com/questions/19032296/how-to-use-git-revert

git log

git log --oneline

git revert <versionId>
git reset <versionId> 
```

✔️💚 [cheatSheet](https://drive.google.com/file/d/1K7P-qvJ7fo_zg2ntea9bRxCHorhtiyhr/view?usp=sharing)

♻️ @ Created by Parth with 💚



