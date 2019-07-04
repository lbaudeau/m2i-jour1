[https://fr.atlassian.com/git/tutorials/setting-up-a-repository](setting up a repository)
--------------------------------------------------------------------------------------------------------------------------
# Configurer git :  `git config`

```bash
git config user.email
git config "user name"

```







# Créer un dépôt

## Initialisation d'un nouveau dépôt : `git init`

Pour créer un nouveau dépôt, utilisez la commande `git init`. 
`git init` est une commande unique que vous utilisez durant la configuration initiale du nouveau dépôt. 
Lorsque vous exécutez cette commande, un nouveau sous-répertoire .git est créé dans votre répertoire de travail courant. 
De même, une nouvelle branche master est créée. 

### Contrôle de version d'un projet existant avec un nouveau dépôt Git

```bash
cd /path/your/existing/project/
git init
```

ou si vous desirez créer un nouveau depot local : 

```bash
git init <répertoire de votre projet>
```

# Cloner un dépôt existant : `git clone`

```bash
git clone <URL_dépôt>
```
Cette commande récupère la dernière version des fichiers du dépôt distant sur la branche master et les ajoute à un nouveau dossier.




# Enregistrer des changements dans le dépôt : `git add` et `git commit`

Redéfinissez les répertoires sur /path/your/existing/project/
Créez un nouveau fichier Hello-world.txt.txt avec pour contenu ~"contenu test pour le tutoriel Git"~
Ajoutez le fichier Hello-world.txt à la zone de staging du dépôt avec la commande git add
Créez un nouveau commit ; son message doit décrire le travail effectué dans le commit

```bash
cd /path/your/existing/project/
echo "Contenu Hello-world pour le tutoriel Git" >> Hello-world.txt
git add Hello-world.txt
git commit -m "Hello-world.txt ajouté au dépôt"
```


# Collaboration dépôt à dépôt : `git push`



# Créer des branches

git branch : liste des branches

git branch b01  : creaton branche 01

git checkout -b b03 : creation de la branche b03, se positionne dessus 

