1. CHECK GLOBAL SETTINGS
git config --global --list 

1.1. INITIALIZE AUTHOR'S NAME AND ADDRESS IF NOT SPECIFIED
git config --global user.name "NAME"
git config --global user.email "EMAIL"

1.2. CHECK CHANGES IN GLOBAL SETTINGS
git config --global --list

2. INITIALIZE A REPO
git init

3. ADD FILES TO THE REPO
git add .

4. COMMIT THE REPO
git commit -m "COMMIT MESSAGE"
OR
git commit -am "COMMIT MESSAGE"

5. CHECK REPO'S STATUS
git status

5.1. CHECK COMMIT LOGS
git log
OR
git log --oneline
OR
git log <file-name>
OR
git log <since>..<until>
OR
git log -n <limit>
