# GitCommands

git

##Commit normal, o segundo commit 
git add .
git commit -m “message”
git pull - -rebase <remote> <branch>
	git status
	git add .
	git rebase - -contine
git push <my remote> <branch> - -force (force is optional)

##Commit amend (to have only one commit)
git add .
git commit - -amend
git pull - -rebase <remote> <branch>
	git status
	git add .
	git rebase - -cbrontine
git push <my remote> <branch> - -force

##Ver branches y remotes
git remote
git branch -vvl

##Renombrar Branch
git branch -m <newname>
git branch -m <oldname> <newname>

##Rename Remote
git remote rename origin destination

##Borrar Branch
git branch -D bugfix

##Cortar un nuevo branch
git pull <remote> <branch> (o solo git pull si est’a apuntando a un remoto)
git checkout -b <new-branch>

-Merge a branch directo
git pull <remote> <branch>

##Force a brand to a different state (you’ll lose your changes)
git fetch <remote>
git reset - -hard <remote>/<branch>

##Para ver la historia de local 
git reflog
git reflow <remote>

##Para tracker
git branch -u <remote>/<branch>

##Jalar un branch nuevo y trackearlo
git checkout -b O_Master live/master

##CLONANDO REPOSITORIO
git clone git@github.paypal.com:Customers-R/node-manage-credentials.git
git remote rename <oldname> <newname>
fork the repo to your local repository
###dd local repo to machine folder…
git remote add najash git@github.paypal.com:nguluarte/merchantcardnodeweb.git

##Track a new branch
git checkout -t origin/develop

##Para ver los remotos
git remote  -v

##Commit sin test (githooks)
-git commit -m “asda”  - -no-verify

## Delete untracked files
git clean -df

##Regular fetch merge
git fetch upstream
git merge upstream/develop

## Reset 
git reset —hard
git fetch origin develop
git reset —hard origin/develop
