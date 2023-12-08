## Contribuer à ToDo & Co
## Introduction
## Merci de prendre le temps de contribuer !

Ce fichier est un ensemble de directives pour contribuer à l'amélioration de l'application ToDo & Co. Suivre ces directives aide à communiquer que vous respectez le temps des développeurs qui gèrent et développent ToDo & Co. En retour, ils devraient réciproquer ce respect en traitant votre problème, en évaluant les changements et en vous aidant à finaliser vos demandes de fusion (pull requests).

## Code de conduite
Utiliser un langage accueillant et inclusif
Respecter les différents points de vue et expériences
Respecter tous les points de vue et être ouvert aux opinions diverses
Accepter de manière constructive les critiques
Orienter son intention vers ce qui est le mieux pour la communauté
Garder à l'esprit qu'il s'agit d'un travail d'équipe

## Comment contribuer
Fourchez le dépôt (repo).
Installez le projet localement
Si ce n'est pas déjà fait, installez le projet sur votre machine via Git, en suivant les instructions d'installation dans le fichier Readme.
Créez une nouvelle branche, en veillant à la nommer de manière cohérente et compréhensible (de préférence en anglais), par exemple feature-foo ou bugfix-bar.
Effectuez vos modifications de code, en les divisant en plusieurs commits si nécessaire. Rédigez les messages de commit de préférence en anglais.
Testez vos modifications. Privilégiez l'ajout de nouveaux cas de test plutôt que la modification de ceux existants.
Exécutez les tests pour vérifier qu'ils passent toujours après vos modifications : make test
Ensuite, mettez à jour le fichier de couverture de test pour Codacy, avec la commande suivante :
bash <(curl -Ls https://coverage.codacy.com/get.sh) report -r reports/clover.xml
Poussez vos modifications et créez une demande de fusion (pull request).
Plus de détails sur les PR dans la documentation GitHub.

## Si votre contribution est approuvée, elle sera fusionnée dans la branche principale (main) du projet.

## Merci d'avance pour votre contribution !
