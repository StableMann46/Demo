# Demo
Notes were taken from the YouTube channel Apana Collage. Link here: "https://youtu.be/Ez8F0nW6S-w?si=bLC4poHgQO_9kXC9"
Using git with VS code: Article with good information. Link here: "https://www.gitkraken.com/blog/vs-code-git#prerequisites-to-using-git-in-vs-code"

<h2>Topic 01: Conventions: </h2>
Repository meaning folder.
Commit chnages means pushing updated code/text.
` Tilda means we are currently in our root directory.
pwd means present working directory
cd means change directory
mkdir make new directory
ls list all files in pwd
ls -a to see all hidden files
In VS code we have 4 types of status changes. M = Modified (changed) U = Untracked (Means we created a file that Git does not know yet) Staged = file is ready to commit. And last is Unmodified = Means unchanged.
git add . makes add for all the files in repo.

<h2> Topic 02: Configuring Git </h2>
We do it using the command "git config" 
There are two types of configuration: One is global level -- changing the full system using one email address. Another is the Local level -- let's say we have a project and specific repository -- changing that using another email address.

This is to set username<br>
git config --global user.name "My name"

To set email address<br>
git config --global user.email "abcd@gmail.com"

To see the chnages we just did <br>
git config -- global --list

<h2> Topic 03: Clone and Status </h2>
Clone is used for cloning a repo on our local machine <br>
Command: git clone <- some link ->
HTTPS is recommended for cloning repos as it is beginner-friendly. You can also use SSH.

Status: displays the state of the code. <br>
command: git status
File ko vs me modified karne ke badd hamara 2 step process hota he. one is add and other is commit.
Jab tak hum ye nahi karte tab tak vs code hame M as modified files dikhayega

<h2> Topic 04: Add and Commit </h2>
add: adds new or changed files in your working directory to the Git staging area.
Command: git add <- file name ->

commit: it is the record of change.
Command: git commit -m "some message"
Here -m is for message.

Your branch is ahead of 'origin/main' by 1 commit. Means the new files will notbe visible to Github.
To do that we use push command.
push: uplaod local repo content to remote repo
Command: git push origin main

