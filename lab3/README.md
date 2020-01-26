# Lab 3

1- Dans cet atelier, vous allez travailler sur quelques exemples simples de mise à jour de fichiers dans la working area et dans la staging area.

```shell script
$ git status
$ git status –s
```
2- Creer un nouveau fichier et verifier son etat
```shell script
$ echo content > file3.c
$ git status
$ git status –s
```
**Question:**   
Est-ce que ce fichier est tracked ou untracked?

3- Stage ce fichier et verifiez son etat.
```shell script
$ git add .   (or git add file3.c)
$ git status   (git status –s if you want)
```

**Questions:**
Est-ce que ce fichier est tracked ou untracked?
Que signifie Changes to be committed ?

4- Editez le meme fichier et verifier son etat.
```shell script
$ echo change > file3.c
$ git status
````
**Questions:**
Pourquoi voyez-vous le fichier répertorié deux fois?  
Où se trouve la version répertoriée comme modifications à valider (dans le répertoire de travail, la zone de transit ou le référentiel local)?  
Où se trouve la version répertoriée comme Modifications non transférées pour la validation (dans le répertoire de travail, la zone de transit ou le référentiel local)?  

5- Faites un diff entre la version entre la staging area .  
````$ git dif````

6-Continuez et verifier l'etat
$ git commit –m "my comment"
$ git status

**Questions**:  
Quelle version avez-vous validée: celle de la zone de transfert ou celle du répertoire de travail?

7- Stage the modified file you have in your working directory and do a status check.
```shell script
$ git add .
$ git status
````
8- Modifiez le fichier dans le répertoire de travail une fois de plus et effectuez une vérification d'état.
```shell script
$ echo "change 2"> file3.c
$ git status
```
À ce stade, vous avez une version du même fichier dans le référentiel local (celui que vous avez validé à l'étape 6), une version dans la zone de transfert 
(celle que vous avez transférée à l'étape 7) et une version dans le travail