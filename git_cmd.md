## Git Commands

### Git Config 

```sh
git config --list    #get the config username for the repo
git config user.name  #get the repos settings
git config --global --list  #get 
~/.gitconfig  #check the git config file
git config --global user.name "Alvin J. Alexander"   #change the git user name globally, remove global it will do locally 
git config --global user.email [your email address here]  #change for the user email globally 
```

### For pushing

```bash
git add .
git add fil*   #aadd the file with starting fil
git commit -m "name"
git push
```

### For Pulling and Force Pulling

```bash
git pull
git push --force
git reset --hard HEAD
git fetch --all
```

### Git init

```bash
git init
git remote add origin <the git url>
git push -u origin master
```

### Misc Commands

```sh
git status   #to check the branh
git log --stat   #to show the commit logs
git commit --amend   #allows you to modify and add changes to the most 
git branch branch_name  # With this command, you can create a new branch. 
git checkout branch_name  #to change the branch
git branch  #git branch list 
git checkout -b branch_name   #to make a branch and check out that one 
```





### Links 

```
https://www.freecodecamp.org/news/git-cheat-sheet/
```

