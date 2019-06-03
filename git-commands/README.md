In the git logs window appears on the console, just hit the 'q' key to quit.

##### Create a Git repository in the current directory.
```bash
$> git init
```
 
##### Add a file into the stage area.
```bash
$> git add
``` 
##### Add the whole changed files into the stage area.
```bash
$> git add .
```
 
##### Commitar é ...
```bash
$> git commit -a [-m 'your commit message']
```

##### Identify the repository commit history.
```bash
$> git log
```

##### I don't do git log all the time, but when i do just remember (A DOG).
```bash
$> git log --all --decorate --oneline --graph
```

##### List your Git configurations.
```bash
$> git config --list
```

##### Oups, I missed to add this file to my commit... thanks Git for the `--amend`.
```bash
$> git commit -m 'It's all here'
$> git add index.html
4> git commit --amend
```

##### Redoing a changed file for how it was in the previous commit.
```bash
$> git reset HEAD README.md
```

##### How to discard the changes I've made.
```bash
$>git checkout -- bird_noises.avi
```

##### Send to branch `-dev` all files in the stage are.
```bash
$> git push origin Bodera-git-dev 
```

##### Colete do servidor master todas as informações e clone neste diretório
```bash
$> git pull origin master
```

##### Create the branch on your local machine and switch in this branch
```bash
$> git checkout -b [name_of_your_new_branch]
```

##### Push the branch on github. Assuming that `origin` is your target.
```bash
$> git push origin [name_of_your_new_branch]
```

##### You can see all branches created by using. Assuming that `origin` is your target.
```bash
$> git branch
```

##### In order to delete a __local__ branch. Assuming that `origin` is your target.
```bash
$> git branch -d [the_local_branch]
```

##### In order to delete a __remote__ branch. Assuming that `origin` is your target.
```bash
git push origin --delete [the_remote_branch]
```

##### Sometimes is important to synchronize your branch list. The `-p` stands for ``--prune`, means that before fetching, remove any remote-tracking references that no longer exist on the remote
```bash
git fetch -p
```