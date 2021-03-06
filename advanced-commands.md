### CHECK SYSTEM SETTINGS
+ git config --system --list 

### CHECK REPOSITORY-SPECIFIC SETTINGS
+ git config --local --list 

### CHECK FILE SETTINGS
+ git config --file --list 
+ git config --f --list 

### UNSET SETTINGS
+ git config _--global_ --unset _SECTION-NAME.SECTION-VARIABLE_

### START THE SSH AGENT
+ eval "$(ssh-agent -s)"

### ADD THE SSH PRIVATE KEY TO THE SSH_AGENT ON MAC OS 
+ ssh-add -K _LOCATION-OF-THE-GENERATED-KEY_

### COPY THE CONTENTS OF THE PUBLIC SSH KEY TO THE CLIPBOARD ON MAC OS/UNIX
+ pbcopy < _PATH-TO-THE-PUBLIC-KEY_

### EXAMINING THE DIFFERENCE OF A SPECIFIC FILE OR DIRECTORY
+ git diff -- _PATH-TO-A-FILE-OR-A-DIRECTORY_
+ git diff _COMMIT-HASH_ -- _PATH-TO-A-FILE-OR-A-DIRECTORY_

### COMPARING THE INDEX TO AN ARBITARY COMMIT 
+ git diff --cached _COMMIT-HASH_
+ git diff --cached _COMMIT-HASH_ -- _PATH-TO-A-FILE-OR-A-DIRECTORY_

### COMPARING COMMITS AND BRANCHES
+ git diff _COMMIT-HASH-OR-BRANCH-NAME_ _COMMIT-HASH-OR-BRANCH-NAME_
+ git diff _COMMIT-HASH-OR-BRANCH-NAME_ _COMMIT-HASH-OR-BRANCH-NAME_ -- _PATH-TO-A-FILE-OR-A-DIRECTORY_ 
+ git diff _COMMIT-HASH-OR-BRANCH-NAME_.._COMMIT-HASH-OR-BRANCH-NAME_
+ git diff _BRANCH-A_..._BRANCH-B_ -- _PATH-TO-A-FILE-OR-A-DIRECTORY_

