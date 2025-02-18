# All Git Commands
1. Notes were taken watching YouTube video from Apana Collage.  
"https://youtu.be/Ez8F0nW6S-w?si=bLC4poHgQO_9kXC9"  
2. Article showing instructions for using git in VS code and other important information.  
"https://www.gitkraken.com/blog/vs-code-git#prerequisites-to-using-git-in-vs-code"


## Topic 01: Conventions
* Repository meaning folder
* Commit chnages means pushing updated code/text
* Tilda means we are currently in our root directory
* `pwd` means present working directory
* `cd` means change directory
* `mkdir` make new directory
* `ls` lists all files in pwd
* `ls` -a to see all hidden files
* `git add .` makes add for all the files in repo
* In VS code we have 4 types of status changes. M = Modified (changed) U = Untracked (Means we created a file that Git does not know yet) Staged = file is ready to commit. And forth is Unmodified = Means unchanged.


## Topic 02: Configuring Git
* Use command `git config`
* Two types of configuration. One is global level - changing the full system using one email address. Another is the Local level - for a project and specific repository - changing that using another email address.

> Command to set username  
`git config --global user.name "My name"`  

> Command to set email address  
`git config --global user.email "abcd@gmail.com"`

> Command to see the chnages we did  
`git config -- global --list`


## Topic 03: Clone and Status
* Clone is used for cloning a repo on our local machine
  > Command to clone  
  `git clone <- some link ->`
* HTTPS is recommended for cloning repos as it is beginner-friendly. You can also use SSH.
* Status displays the state of the code
  > command to check status  
  `git status`
* File ko vs me modified karne ke badd hamara 2 step process hota he. one is add and other is commit
* Jab tak hum ye nahi karte tab tak vs code hame M as modified files dikhayega


## Topic 04: Add and Commit and Push
* add basically adds new or changed files in your working directory to the Git staging area
  > Command for add is  
  `git add <- file name ->`
* Commit is the record of change
  > Command to commit chnages. Here -m is for message.  
  `git commit -m "some message"`
* Receving this message "Your branch is ahead of 'origin/main' by 1 commit" means the new files will not be visible to Github. To achieve we use push command.
* push means uplaod the content of local repo to remote repo
  > Command to push is  
  `git push origin main`


## Topic 05: Init
Github ke upar jo repo he voh origin he
Projects local machine me banate he fir hum use github pe push karte he 
Start it with git init

* init is used to create a new git repo
  ```
  git init
  git remote add origin <-link->
  git remote -v
  git branch
  git branch -M main
  git push origin main
  ```
* Git repo or not -- If there is no hidden folder named git -- after doing ls -a
* we do git init
* now do ls -a. This is git repo now
* check git status
* git commit -m "initial files"
* git status
* All the chnages were made to our local
* now make a repo in github to push our local
  > Before doing push run this command
  `git remote add origin <-link->`
  create remote repo and name it origin
* To verify remote `git remote -v`
* To check branch `git branch`
* Pehle master branch default hoti thi ab usk naam github ne badal ke ==main== kar dia he
* `git branch -M main`
* now we can do `git push origin main`
* or `git push-u origin main` for all times in future. After setting this run only `git push` afterwards
*  jab bhi hum naya project banaye git hub pe banaye fir local me clone kare voh aasan rehta he.


# Workflow --> when working with local git
Github repo --> Clone --> Changes --. Add --> Commit --> Push 

# Git Branches
Ek product me naye features dalne he to tab ye kam aata he
One person is working on one feature and another on another feature. When other developers conmplete developing the feature. We finally merge all the changes.
**branch Commands**
  ```
  git branch // to check branch
  git branch -M main // to rename branch
  git checkout <-branch name-> // to nevigate
  git checkout -b <-new branch name-> // to create new branch
  git branch -d <-branch name-> // to delete branch
  ```
  > feature 1 ke andar chnages karna chahte he.
  `git push origin feature1`
* Ab ham featurea ko main ke sath merge kar de
* Two types 1. using git -- compare two files `git diff <-branch name->` and then merge `git merge <-branch name->`
* 2nd way is using Pull request. Create a PR. Bahoot sare kam kare aur sare developer ka code ek sath main branch me merge kar de.

Now to update chnages from github to our local repo.
Command: `git pull origin main`

Resolving merge conflict -- same jagah ek branch ne change kia aur desre ne same usi jagah change kia. Ab git isko resolve nahi karega. Hum karenge.
`git merge main`

Vs will give us option 1. Accept change....line aayegi
vs code ke sari ajeeb si line aayi he use hata de.
Resolve in Merge Editor

# Another topic: Undoing Chnages

Case 1: Staged changes -- chnages add ho chuke he magar commit nahi hue he.
* Now to reset the changes `git reset index.html` for one file only otherwise `git reset`

Case 2: galti se koi change commit kar dia.
`git reset HEAD~1`
* Iska matlab head ko reset kar do 1 step
* `git log` karke sare commit ko check kar sakte he. To check the history

Case 3: commited changes for (multiple commits)
* `git reset <-commit hash->`
* `git reset --hard hash` vs code aur git dono mese change hat jayega.


# Another topic: Fork -- is a rough copy of our project. And then pull request. Do all the changes in our github account and then merge it with actual project code.
