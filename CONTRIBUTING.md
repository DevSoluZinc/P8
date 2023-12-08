# Contribution à ToDo & CO

## Introduction

Merci d'avance pour votre contribution !

Ce fichier représente un ensemble de lignes directrices pour contribuer à l'amélioration de ToDo & Co App.
Suivre ces directives aide à communiquer que vous respectez le temps des développeurs qui gèrent et développent ToDo & Co App. En retour, ils devraient témoigner du même respect en traitant votre problème, en évaluant les modifications et en vous aidant à finaliser vos demandes de fusion (pull requests).

## Code de conduite

- Utilisation d'un langage accueillant et inclusif
- Respect des différents points de vue et expériences
- Considération de toutes les perspectives et tolérance envers les opinions moins partagées
- Acceptation constructive des critiques
- Focalisation de vos intentions sur ce qui est le mieux pour la communauté
- Garder à l'esprit qu'il s'agit d'un travail d'équipe

## Comment contribuer

1. **Faites un** fork du [dépôt](https://github.com/DevSoluZinc/P8).
2. **Installez** le projet localement : Si ce n'est pas déjà fait, installez le projet sur votre machine via Git, en suivant les instructions d'installation dans le [fichier Readme](Readme.md).
3. **Créez une nouvelle branche**, en veillant à la nommer de manière cohérente et compréhensible (de préférence en anglais), par exemple `feature-foo` ou `bugfix-bar`.
4. **Effectuez** vos **modifications de code**, en les divisant en plusieurs commits si nécessaire. Rédigez les messages de commit de préférence en anglais.
5. **Testez** vos modifications : Privilégiez l'ajout de nouveaux cas de test plutôt que la modification des existants. Exécutez les tests pour vérifier qu'ils passent toujours après vos modifications : ``make test``
6. Ensuite, **mettez à jour le fichier de test de couverture** pour Codacy avec la commande suivante : 
   ```bash
   bash <(curl -Ls https://coverage.codacy.com/get.sh) report  -r reports/clover.xml
