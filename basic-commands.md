### 1. CHECK GLOBAL SETTINGS
+ git config --global --list 

### 1.1. INITIALIZE AUTHOR'S NAME AND ADDRESS IF NOT SPECIFIED
+ git config --global user.name _NAME_
+ git config --global user.email _EMAIL_

### 1.2. CHECK CHANGES IN GLOBAL SETTINGS
+ git config --global --list

### 2. GENERATE SSH KEY
+ ssh-keygen -t rsa -b 4096 -C _KEY-NAME_

### 2.1. AUTHENTICATE SSH KEY
+ ssh -vT git@github.com
+ OR
+ ssh -T git@github.com

### 2.2. ESTABLISH SSH-CONNECTION
+ git remote set-url origin *ssh-link*

### 2.3 RE-ESTABLISH HHTP-CONNECTION
+ git remote set-url origin *http-link*

### 3. INITIALIZE A REPO
+ git init

### 4. ADD FILES TO THE REPO
+ git add .
+ OR
+ git add _FILE-NAME_

### 5. COMMIT THE REPO
+ git commit -m _COMMIT-MESSAGE
+ git commit -am _COMMIT-MESSAGE_

### 6. CHECK REPO'S STATUS
+ git status

### 6.1. CHECK COMMIT LOGS
+ git log
+ git log --oneline
+ git log --oneline --decorate --graph
+ git log --oneline --decorate --graph --all
+ git log _FILE-NAME_
+ git log _SINCE...UNTIL_
+ git log -n _LIMIT_
  
### 7. CLONE A REPO
+ git clone _URL_

### 8. COORDINATE LOCAL AND REMOTE REPOS
+ git remote add origin _URL_
+ git remote show origin
+ git remote -v
  
### 9. PUSH CHANGES
+ git push -u origin master

### 10. PULL CHANGES
+ git pull

### 10.1. PULL WITH REBASE
+ git pull --rebase origin _BRANCH-TO-PULL-FROM_
