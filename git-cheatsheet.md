#general info
Immer auf Branch arbeiten, nicht auf Main, weil sonst vergessen werden kann, Zwischenstände hochzuladen, sodass bei einem Pull Request von Branch auf Main eine Fehlermeldung angezeigt werden kann. Dann --> git pull --rebase, git push

#see all main and branches
git log --graph
extension: Git Graph

#go back to main branch again
git checkout main
git switch <branch/name> //switch from branch to other branch

#create new branch
git branch <new file name, e.g. fix/recovery>

#switch to a former version
git checkout <version number>
git restore . or <filename>

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
8. git push origin main or git push origin <branch/name> //nur wenn auf remote gespeichert werden soll

- when new file: repeat no. 6-8

#leeren Ordner als Git commiten
touch .gitkeep
git add .
git commit -m "add testfolder"
