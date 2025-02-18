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


## Topic 04: Add and Commit
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

Video paused at 39:58


