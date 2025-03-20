Réponses aux questions du TP3
Réponses TP3 :

-Exercice1 :
-1. Si on tente de supprimer une brache sur laquelle vous êtes actuellement, Git renverra un message d'erreur indiquant qu'il est impossible de supprimer une branche active. Pour résoudre cela, on doit d'abord se déplacer sur une autre branche avec la commande "git checkout <la branche en question>" et ensuite on pourra supprimer la branche souhaitée.
-2. On peut utiliser la commande suivante pour afficher les différences : "git diff main.. feature-1". Cela montre les différentes spécifiques entre les fichiers et les changemets réalisés dans chaque branche.


-Exercice3 :
-1. Quand on tente de fusionner conflit-test dans main, un conflit est survenu parce que les deux branches modifiaient a même ligne du fichier README.md. Pour résoudre le conflit, on doit modifié le fichier pour inclure les deux versions : #Projet d'exercice - Version Main et Test . Ensuite on ajoute le fichier résolu avec : "git add README.md, puis finalisé la fusion avec git commit -m "Résolution de conflit"
-2. Cela veut dire combiner les modifications des deux branches dans le fichier final, de manière à conserver toutes les informations pertinentes. C'est une solution manuelle, ou on décide des parties à garder ou modifier.

-Exercice4 :
-1. Après le rebase, tous les commits de la branche feature-rebase ont été réappliqués sur la branche main comme s'ils avaient été créés après les commits de main. L'historique est ainsi rendu linéaire,sans divergences.
-2. Une fusion (merge) conserve l'historique des branches en créant un commit de fusion, ce qui peut inclure des bifurcations dans l'historique. Alors que un rebase réapplique les commit branche sur un autre, créant un historique linéaire plus propre, mais modfie l'ordre des commits.

-Exercice5 :
-1. Les commandes recommandées pour visualiser l'historique sont : "git log --all --decorate --oneline --graph" ou si on configure l'alias : git adog.
-2. "git branch --merged" :liste les branches qui ont déjà été fusionnées dans la branche active. alors que "git branch --no-merged" :liste les branches qui n'ont pas encore été fusionnées dans la branche active.
