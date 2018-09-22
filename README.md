### QUICK TIPS
+ Pull before push
+ Diff before merge

### 1. CHECK GLOBAL SETTINGS
+ git config --global --list 

### 1.1. INITIALIZE AUTHOR'S NAME AND ADDRESS IF NOT SPECIFIED
+ git config --global user.name "NAME"
+git config --global user.email "EMAIL"

### 1.2. CHECK CHANGES IN GLOBAL SETTINGS
+ git config --global --list

### 2. INITIALIZE A REPO
+ git init

### 3. ADD FILES TO THE REPO
+ git add .

### 4. COMMIT THE REPO
+git commit -m "COMMIT MESSAGE"
+ OR
+ git commit -am "COMMIT MESSAGE"

### 5. CHECK REPO'S STATUS
+ git status

### 5.1. CHECK COMMIT LOGS
+ git log
+ OR
+ git log --oneline
+ OR
+ git log --oneline --decorate --graph
+ OR
+ git log --oneline --decorate --graph --all
+ OR
+ git log *file-name*
+ OR
+ git log *since*..*until*
+ OR
+ git log -n *limit*
  
### 6. CLONE A REPO
+ git clone *url*

### 7. COORDINATE LOCAL AND REMOTE REPOS
+ git remote add origin *url*
+ git remote show origin
+ git remote -v
  
### 8. PUSH CHANGES
+ git push -u origin master

### 9. PULL CHANGES
+ git pull

### 9.1. PULL WITH REBASE
+ git pull --rebase origin *branch-to-pull--from*

### 10. FETCH CHANGES
+ git fetch
+ git merge

### 11. CHECK EXISTING BRANCHES
+ git branch
+ OR
+ git branch -a

### 11.1. CREATE A NEW BRANCH
+ git branch *name*
+ OR
+ git checkout -b *name*

### 11.2. SWITCH TO ANOTHER BRANCH
+ git checkout *branch-name*

### 11.3. RENAME A BRANCH
+ git branch -m *old-name* *new-name*

### 11.4. DELETE A BRANCH
+ git branch -d *name*
+ git branch -D *name*
  
### 12. COMPARE BRANCHES
+ git diff *branch1* *branch2*

### 13. MERGE BRANCHES
+ git merge *branch-to-merge-with*
+ git merge *branch-to-merge-with* --no-ff
+ git merge *branch-to-merge-with* -m "MESSAGE"

### 14. REBASE
+ git rebase *branch-to-rebase-to*
  
### 15. GENERATE SSH KEY
+ ssh-keygen -t rsa -b 4096 -C "KEY NAME"

### 15.1. AUTHENTICATE SSH KEY
+ ssh -vT git@github.com
+ ssh -T git@github.comyes

### 15.2. ESTABLISH SSH-CONNECTION
+ git remote set-url origin *ssh-link*

### 15.3 RE-ESTABLISH HHTP-CONNECTION
+ git remote set-url origin *http-link*

### 16. FILE DELETION
+ git rm *file-name*
+ git rm --cached *file-name*
+ git clean -fd

### 17. FILE RENAMING
+ git mv *old-file-name* *new-file-name*

### 18. FILE RELOCATION
+ git mv *old-file-name* *new-directory-name*

### 19. UNSTAGING
+ git reset HEAD *file-name*

### 19.1. DISCARD CHANGES
+ git checkout --*file-name*
