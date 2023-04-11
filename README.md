Nom : Pavlova

Groupe : A1

Année : 2022/2023

IUT Le Havre - Cours GIT

# Compte-rendu TP 3 : Travailler en équipe sur un depôt github distant

Dans ce deuxième TP, on apprend à travailler en équipe.

***

## Inviter des  collaborateurs dans un dépôt personnel

Pour commencer, un membre de l'équipe, que nous appellerons *Athos*, créera un dépôt sur son compte github appelé tp3 avec les mêmes paramètres que tp2.
Une fois le dépôt créé, allez dans **Settings**, puis **Manage Access** et à la fin **Invite a collaborator**.

Demandez à votre collègue (que nous appellerons *Portos*) son nom d'utilisateur GitHub et invitez-le à accéder à votre dépôt.

***

## Gérer des nouvelles fonctionnalités à l’aide des branches

Supposons que nous ayons des "ramifications" dans les idées et la mise en œuvre du projet, ou que nous voulions tester une fonctionnalité dans une autre branche avant de l'intégrer dans la branche principale.
Pour ce faire, nous pouvons travailler dans une nouvelle branche.

Avec la commande `git branch` vous pouvez savoir sur quel branche vous êtes.

Avec la commande `git checkout -b test`, vous pourrez crée et vous deplacer sur la branche test.

*L'option -b permet de dire à **checkout** que nous créons et nous déplacons sur la branche*

Pour se déplacer de branche en branche, vous avez juste à utiliser la commande `git checkout nomBranche`

***Remarque : lorsque vous crée des fichier dans les branches (par exemple la branche test), ils ne seront pas visible par la branche main.***

Si vous voulez suivre le développement depuis la branche princiaple, tappez la commande :

`git log --graph --oneline --all --decorate --topo-order`

***

## Fusionner la branche de test dans la branche principale

Si vous voulez merger deux branches, par exemple, main et test, aller tous dabord sur la branche main puis tapper la commande :
`git merge test`

Vous pouvez voir maintenant avec la commande `ls` tous les fichiers de main et de test 



