#creating local repositories
cd path/to/my/folder
git init

#check status
git status

#committing in a local repository
git add <filename> (without brackets)
git commit -m "add foo"
git log

#returning to last committed state or to individual files
git restore .
git restore <filename>

#connecting to remote repository

1. create new empty repo on GitHub
   git remote add origin <ssh url>
   git push origin main

#cloning a remote repository (from GitHub to local)
git clone <ssh url>

#synchronizing local & remote repositories
git push //upload content to remote repo
git pull //download content from the remote repo

#check connection
git remote -v

e.g. creating new folder local --> create local git --> create remote git on GitHub

1. #create new folder with new files
2. cd path/to/my/folder
3. git init
4. #create new repo on GitHub
5. git remote add origin <ssh url>
6. git add <filename> or git add .
7. git commit -m "add foo"
8. git push origin main

- when new file: repeat no. 6-8
