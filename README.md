# exercice3



EXERCICE n°3 :
Vous allez créer un nouveau projet sur votre dépot git.
Vous allez appeler votre projet “exercice3”.
Ci-dessous les étapes à effectuer :
● En local, vous allez créer un projet que vous allez appeler
exercice3.
● Dans cet exercice, vous aurez besoin d’utiliser :
○ git branch “nom de la branche” : pour créer une
branche dans votre projet.
○ git checkout “nom de la branche” pour vous déplacer
vers une branche.
● Vous allez créer un fichier texte qui va s’appeler
“fichier_branche_master” et qui va contenir le texte, “bonjour,
je suis le fichier de la branche master”.
● Vous allez ensuite pousser ce fichier sur votre dépôt distant
sur la branche “master”.
● Vous allez ensuite créer une branche que vous allez appeler
avec “votre prenom” (avec la commande git branch).
● Vous allez vous positionner sur cette branche (en utilisant la
commande git checkout “nom de votre branche”).
● Vous allez créer un nouveau fichier qui va s’appeler
“fichier_branche_votre_prenom”et qui va contenir le texte,
“bonjour, je suis le fichier de la branche votre prenom”.
● Vous allez ensuite pousser ce fichier sur votre dépot distant
mais sur votre nouvelle branche “votre prenom”.
A la fin, vous aurez, 2 branches, et chacune de ces branches
devraient contenir un seul et unique fichier.

voici les commandes que j'ai effectué pour l'exercice : 

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3
$ echo "# exercice3" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/karimm59200/exercice3.git
git push -u origin main
Initialized empty Git repository in C:/Users/karim/OneDrive/Bureau/exercie3/.git/
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it
[master (root-commit) da7d532] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 218 bytes | 218.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/karimm59200/exercice3.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (main)
$ git checkout -b master
Switched to a new branch 'master'

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fichier_branch_master

nothing added to commit but untracked files present (use "git add" to track)

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (master)
$ git add fichier_branch_master

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (master)
$ git commit -m "fichier modif"
[master 871f3f5] fichier modif
 1 file changed, 1 insertion(+)
 create mode 100644 fichier_branch_master

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (master)
$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (master)
$ git push origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 6 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 326 bytes | 326.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/karimm59200/exercice3/pull/new/master
remote:
To https://github.com/karimm59200/exercice3.git
 * [new branch]      master -> master

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (master)
$ git checkout -b karim
Switched to a new branch 'karim'

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (karim)
$ git status
On branch karim
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fichier_branch_karim

nothing added to commit but untracked files present (use "git add" to track)

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (karim)
$ git add fichier_branch_karim

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (karim)
$ git commit -m "fichier branche karim"
[karim 7378b31] fichier branche karim
 1 file changed, 1 insertion(+)
 create mode 100644 fichier_branch_karim

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (karim)
$ git push
fatal: The current branch karim has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin karim

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (karim)
$ git push origin master
Everything up-to-date

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (karim)
$ git push origin karim
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 6 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 359 bytes | 359.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'karim' on GitHub by visiting:
remote:      https://github.com/karimm59200/exercice3/pull/new/karim
remote:
To https://github.com/karimm59200/exercice3.git
 * [new branch]      karim -> karim

karim@LAPTOP-AV2UFMKP MINGW64 ~/OneDrive/Bureau/exercie3 (karim)
$

git branch - d main pour supprimer main 

j'ai mis la branche master par default pour pouvoir supprimer main. 
