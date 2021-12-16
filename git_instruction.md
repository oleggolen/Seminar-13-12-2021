# Git instruction (local and remote versions)


## What is Git?
---

Git is one of the many ways to realize version control systems. This is the most famous project in the world. There are local and internet services.

# Local commands:

## Repository preparing
---

To prepare repository, open a folder for repository and go to command "**git init**" (the folder will be inicialized. Now there is one more folder with name ".git"). All right, you have repository.


## Switch between commits
---

We can make lot of branch. Then we can go to new branch ahd format documets into the branch and save new data into the branch (the new data will be invisible in other branches). But next time we can merge some branches in one branch (read head Merge).
### add commit:
- First add a file to git ("**git add** 'file name'"). You  can add some more files at once, just type the names and key 'space' between.
- Then type command: "**git commit** -m 'message'". "-m" it means message for other developers, don'b be shy, write more about your commit.
### checkout to commit:
- To go to some point of commit set the commands:
    - Type "git log" command to see hash names of commits
    - Type "git checkout 'five first symbols of commit hash name'"

Other ways to use the command "**git checkout**":
    - "**git checkout** 'branch name'" to switch to the other branch
    - "**git checkout** -b 'new branch name'" - create new branch and go to new branch


## Use some time comand "**git status**" to check current status of git synchronization:
- "**git status**" - show git status about something to save.
- "**git diff**" - show the different between last commit and new data.


## Git log
---

The command "git log" show all of your commits. Also the command has some parametrs:
    - "--oneline" - to see short list of commits
    - "--graph" to see commit's tree. Then press key 'space' to see more graph info.


## Branches
---

We can create some branches to have some ways to working. So we have protection "master" branch from mistakes on other branches.
    Important info:
    Before you switch to some branches you need to save everywere your data on current branch. Or you have a risk loose data from next branch, were you will go.

Use these commands:

- "**git branch**" - show names of branches. Or use the code with command:
    - "**git branch** 'new branch name'" to create new branch
    - "**git branch** -d 'branch name'" - delete the branch


## Merge
---

To merge two branch in one, use command "git merge 'other branch name'". The commad add data from other branch to current branch.

Use like:
- "**git merge** 'branch name'" - to merge data from "branch name" to current branch.


## Delete branch
---

Use "git branch -D 'name branch'" to delete the branch.


# Remote commands:

## Working whit your own repository 

You have two general ways to get remote repository. First is to create a local version and push it on server. Second way is make remote repositoty at server and then pull it to local system.

How to puss.
Make repo as you do it  every time and commit it.
Then you need to go to Github to make there repository (keep it clear, do nothing into Github repo). Copy link and come back to local computer.
Use the command:

- "**git remote** add origin  <REMOTE_URL>" (At first time git will ask you password to connect Github account)

Or use the command, if you want to clone repository from Github:

- "**git clone** <REMOTE_URL>"

Then you can use next commands:

- "**git push** origin master" - to push to Github brench 'master'
- "**git pull** origin master" - tu pull lical copy ti Github.

Warning!
If you have at the same time different commit version in server and local computer, oyu need first run command "**git pull**" to merge two versions, then you will can ri=un "**git push".


## Collaboration:

You can get some other autors repository and add it in your account. Press button **Fork** in home page of the repository. Then clone the repo on your PC.

Make new commits and pull it. Then pres buttom **Pull requests** on Github.


For more infirmation please get GeekBrains course "Developer" and enjoy yourself!
