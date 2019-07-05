# reecriture de l'historique ``git rebase`


permet e réécrire l'historique des N--1 derniers commits ( de preferences non propagés)

git rebase --interactive HEAD~6


=> affiche Vi avec les 6 derniers commits
opptions possible : 
pick    : choix du comit
reword  : modifie le message du commit
edit    : permet de modifier le comit
squash  : ecrasé
fixup   :
exec    :
drop    :
