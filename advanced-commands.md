### CHECK SYSTEM SETTINGS
+ git config --system --list 

### CHECK REPOSITORY-SPECIFIC SETTINGS
+ git config --local --list 

### CHECK FILE SETTINGS
+ git config --file --list 
+ OR
+ git config --f --list 

### UNSET SETTINGS
+ git config _--global_ --unset _SECTION-NAME.SECTION-VARIABLE_

### START THE SSH AGENT
eval "$(ssh-agent -s)"

### ADD THE SSH PRIVATE KEY TO THE SSH_AGENT ON MAC OS 
ssh-add -K _LOCATION-OF-THE-GENERATED-KEY_

### COPY THE CONTENTS OF THE PUBLIC SSH KEY TO THE CLIPBOARD ON MAC OS/UNIX
pbcopy < _PATH-TO-THE-PUBLIC-KEY_
