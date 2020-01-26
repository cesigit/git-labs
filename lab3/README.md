# Lab 3

Dans cet atelier, vous allez travailler sur quelques exemples simples de mise à jour de fichiers dans la working area et dans la staging area.

```shell script
$ git status
$ git status –s
```
Creer un nouveau fichier et verifier son etat
```shell script
$ echo content > file3.c
$ git status
$ git status –s
```
**Question:**   
Est-ce que ce fichier est tracked ou untracked?

Stage ce fichier et verifiez son etat.
```shell script
$ git add .   (or git add file3.c)
$ git status   (git status –s if you want)
```

**Questions:**
Est-ce que ce fichier est tracked ou untracked?
Que signifie Changes to be committed ?

Editez le meme fichier et verifier son etat.
```shell script
$ echo change > file3.c
$ git status
````
**Questions:**
Pourquoi voyez-vous le fichier répertorié deux fois?  
Où se trouve la version répertoriée comme modifications à valider (dans le répertoire de travail, la zone de transit ou le référentiel local)?  
Où se trouve la version répertoriée comme Modifications non transférées pour la validation (dans le répertoire de travail, la zone de transit ou le référentiel local)?  

 Faites un diff entre la version entre la staging area .  
````$ git dif````



