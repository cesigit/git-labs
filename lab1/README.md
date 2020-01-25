# Lab 1
Sur votre disque local, créez un nouveau répertoire et changez-le (cd) en celui-ci.   
Initialisez un nouveau référentiel en exécutant la commande suivante:  
```git init```  
Cette commande crée un nouveau squelette de référentiel git dans un sous-répertoire nommé .git sous le répertoire courant,   
comme indiqué par le message de sortie de la commande. Cela signifie que vous pouvez désormais commencer à utiliser  
d'autres commandes Git dans le répertoire actuel.  
```shell script
$ git config --global user.name "First-name Last-name"
$ git config --global user.email emailAddress@provider
```
creer 2 fichiers
```shell script
$ echo content > file1.c
$ echo content > file2.c
```
Stage ce fichier avec la command add . (vous pouvez les ajouter un a un au lieu d'utiliser le caractere “.”)
```shell script
$ git add .
```
Si vous souhaitez voir comment la commande add modifie le contenu de votre référentiel .git,  
revenez à l'explorateur de fichiers ou au terminal et changez dans le sous-répertoire .git.  
Tout d'abord, notez la présence d'un fichier nommé index. En termes de terminologie de Git,   
vous pouvez penser à l'étape, au cache et à l'index comme signifiant la même chose.  
Ainsi, ce fichier est essentiellement la zone de transit avec des métadonnées qui incluent des valeurs SHA1, des horodatages, etc.  
Ensuite, examinez à nouveau le répertoire des objets. Cette fois, vous voyez un nouveau nom de répertoire à deux caractères.   
Il s'agit en fait du début d'une valeur SHA1. Le fichier à l'intérieur de ce répertoire est nommé avec le reste de la valeur SHA1.
Revenez dans le répertoire de votre projet (le répertoire ci-dessus .git) avant de continuer.

```$ git commit -m "comment string"```
Remarquez la sortie que vous obtenez. Il y a le nom de la branche - la branche par défaut - master,  
 suivi d'un indicateur qu'il s'agit du premier commit (racine) puis des premiers caractères du SHA1 pour le commit.  
 Prenez note de cette valeur si vous effectuez l'étape suivante.
```shell script
  $ echo more >> file1.c
```
```shell script
$ git commit –am "comment string"
```

```shell script
  git gc
```
