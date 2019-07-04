[https://fr.atlassian.com/git/tutorials/setting-up-a-repository](setting up a repository)
--------------------------------------------------------------------------------------------------------------------------

# Configurer git :  `git config`

## Niveaux de configuration et fichiers associés à git config

```bash
git config user.email "votre_email@exemple.com"
git config user.name  "votre_nom"
```
Permet de configurer aussi bien le local que le distant `--local`, `--global` ou `--system`
Par défaut, git config écrira à un niveau local si aucune option de configuration n'est transmise. 
La configuration au niveau local s'applique au contexte dans lequel le dépôt git config est appelé. 
Les valeurs de configuration locales sont stockées dans un fichier situé dans le répertoire .git du dépôt : .git/config

La configuration au niveau global varie en fonction de l'utilisateur, ce qui signifie qu'elle s'applique à un utilisateur du système d'exploitation. 
Les valeurs de la configuration globale sont stockées dans un fichier situé dans le répertoire de base d'un utilisateur. `~/.gitconfig` sur les systèmes Unix et `C:\Users\<nom_utilisateur>\.gitconfig` sous Windows

La configuration de niveau système est appliquée à une machine complète. 
Cela concerne tous les utilisateurs d'un système d'exploitation et tous les dépôts. 
Le fichier de configuration de niveau système réside dans un fichier gitconfig extrait du chemin d'accès à la racine du système. 
Il se trouve dans `$(prefix)/etc/gitconfig` sur les systèmes Unix. 
Concernant les systèmes Windows, ce fichier se trouve dans `C:\Documents and Settings\All Users\Application Data\Git\config` sous Windows XP 
et dans `C:\ProgramData\Git\config` sous Windows Vista ou des versions plus récentes.


```bash
git config --global user.email "votre_email@exemple.com"
```

Cet exemple écrit la valeur `your_email@example.com` pour le nom de configuration user.email. 
Il utilise le flag `--global` pour que cette valeur soit définie pour l'utilisateur actuel du système d'exploitation.


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



# Creation de branche



# Merge Rebase