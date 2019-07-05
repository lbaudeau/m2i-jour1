# le remisage `git stash`

git stash : remise le travail en cours
git stash save "message paralnt svp"

git stash list : liste les remisage en cours
git stash show -p affiche le diff de la remise la plus recente

git stash apply : applique la derniere remise
git stash apply stash@{2} : applique la remise spécifiée


git stash pop : applique et supprime la remise
git stash drop : suppprime la remise la plus recente sans l'appliquer
git stash branch b01 : applique la remise la pluss recente au sein d'une nouvelle branche

