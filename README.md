# Demo
Notes took from YouTuve channel Apana Collage. Link here: "https://youtu.be/Ez8F0nW6S-w?si=bLC4poHgQO_9kXC9"
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
In VS code we have 4 types of status changes. M = Modified (changed) U = Untracked (Means we created a file that Git does not know yet) Staged = file is ready to committed. And last is Unmodified = Means unchanged.
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
HTTPS is recommanded for cloning repos as it is begginer-friendly. You can also use SSH.

Status: displays the state of the code. <br>
command: git status
