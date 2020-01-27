# Lab 4
En commençant dans le même répertoire que vous avez utilisé pour le Lab 3, commencez par apporter une autre modification au référentiel pour rendre l'historique plus intéressant.   
Ajoutez une ligne au premier fichier que vous avez validé dans le référentiel, puis mettez en staged area et committez.  
Notez que vous pouvez utiliser le raccourci suivant:
```shell script
$ echo new >> file1.c
$ git commit -am "add a line"
```
Regardez l'historique que vous avez jusqu'à présent dans votre petit référentiel. Pour ce faire, exécutez la commande log
```shell script
$ git log
$ git status –s
```
Souvent, lorsqu'ils consultent les informations de l'historique Git, les utilisateurs souhaitent uniquement voir la première ligne de chaque entrée, la ligne d'objet. C'est pourquoi il est important de donner un sens à cette première ligne lors de l'utilisation de Git.  
Pour voir uniquement la première ligne de chaque message du journal, vous pouvez utiliser l'option **--oneline**. Essayez-le maintenant.
