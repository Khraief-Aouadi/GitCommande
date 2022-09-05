Liste des commandes GIT
============

### Récupérer & créer un repo GIT

| Command | Description |
| ------- | ----------- |
| `git init` | Met en place le package GIT dans un projet |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Créer une copie du repo distant sur le disque local |

### Les commandes basiques 

| Command | Description |
| ------- | ----------- |
| `git status` | Affiche l'état actuel du repo |
| `git add [file-name.txt]` | Indexe le fichier ciblé |
| `git add -A` | Indéxe tout les fichiers modifié ou non indéxés |
| `git commit -m "[commit message]"` | Valide tout les fichiers (Commit) |
| `git rm -r [file-name.txt]` | Retire un fichier ou un dossier |

### Création de branches & merging de branches

| Command | Description |
| ------- | ----------- |
| `git branch` | Liste les différentes branches ( * Montre la branche courante ) |
| `git branch -a` | Liste des différentes branches (sur le local & sur le dépot distant) |
| `git branch [branch name]` | Créer la branche |
| `git branch -d [branch name]` | Supprime la branche |
| `git push origin --delete [branch name]` | Supprime la branche sur le dépot distant (GitHub) |
| `git checkout -b [branch name]` | Créer une nouvelle branche et l'utilise en branche courante |
| `git checkout -b [branch name] origin/[branch name]` | Clone la branche du dépot distant et l'utilise en branche courante |
| `git branch -m [old branch name] [new branch name]` | Renommer une branche stocké en local |
| `git checkout [branch name]` | Changement de branche |
| `git checkout -` | Change de branche courante pour revenir sur la précédente |
| `git checkout -- [file-name.txt]` | Ignore les modifications apportés au fichier |
| `git merge [branch name]` | Fusionne la branche dans la branche courante |
| `git merge [source branch] [target branch]` | Fusionne la branche source dans la branche cible |
| `git stash` | Deplace les fichiers indéxés dans un dépot temporaire (Stash) |
| `git stash apply` | Récupére les fichiers du dépot temporaire (Stash) et les remets dans votre branche courante |
| `git stash clear` | Supprime tout les fichiers du dépot temporaire (Stash) |

### Partager & mettre à jour son projet 

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Met à jour votre dépot distant (GitHub) à partir du dépot local |
| `git push -u origin [branch name]` | Met à jour votre dépot distant (GitHub) & ajoute la branche courante|
| `git push` | Met à jour le dépôt distant (GitHub) si la branche courante à déjà été ajouté |
| `git push origin --delete [branch name]` | Supprime la branche sur le dépôt distant (GitHub) |
| `git pull` | Importe les derniers changements du dépot distant (GitHub) vers le dépôt local |
| `git pull origin [branch name]` | Importe les derniers changements de la branche |

### Inspection & comparaison 

| Command | Description |
| ------- | ----------- |
| `git log` | Voir les changements  |
| `git log --summary` | Voir les changements (Détail) |
| `git log --oneline` | Voir les changement (Raccourci) |
| `git diff [source branch] [target branch]` | Comparer les changements avant une fusion |
# GitCommande