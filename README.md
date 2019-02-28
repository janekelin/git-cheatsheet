### BEST PRACTICES
+ Pull before push
+ Diff before merge
+ Commit often
+ Commit complete work
+ Write descriptive commit messages
+ Branch extensively
+ Use feature branches
+ Do pull requests
+ Prefer rebase instead of merge commits
+ Version control is not a backup system
+ Don't commit config files
+ Don't create very large repos
+ Run *git clean -n* before *git clean -fd*

### 10. FETCH CHANGES
+ git fetch
+ git merge

### 11. CHECK EXISTING BRANCHES
+ git branch
+ git branch -a

### 11.1. CREATE A NEW BRANCH
+ git branch *name*
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

### 20. DEBUGGING: STRING SEARCH
+ git grep 'STRING'
+ git grep -n 'STRING'

### 20.1. DEBUGGING: EXTRACT INFORMATION ABOUT A KNOWN BUG (AUTHOR AND COMMIT HASH)
+ git blame *file-name*
+ git show *commit-id*

### 20.2. DEBUGGING: IDENTIFYING THE SOURCE COMMITE OF THE BUG
+ git bisect start
+ git bisect good *last-known-good-commit*
+ git bisect bad *last-known-bad-commit*
+ git bisect good
+ git bisect bad
+ git bisect reset
