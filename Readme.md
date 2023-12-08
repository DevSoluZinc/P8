## Prérequis sur votre lieu de travail
#### Serveur
Vous avez besoin d'un serveur web avec PHP7 (>=7.2.5) et MySQL.
Versions utilisées dans ce projet :
- **PHP** 7.4.12
- **MySQL** 5.7.32
Consultez plus d'informations sur les exigences techniques dans la [documentation officielle de Symfony](https://symfony.com/doc/5.4/setup.html#technical-requirements).

#### Frameworks et bibliothèques
Framework : **Symfony** ^6.4.*
Gestionnaire de dépendances : **Composer** ^2.6.5

Pour exécuter les tests, vous avez également besoin de **PHPUnit**. Consultez les exigences dans la [documentation PHPUnit.](https://phpunit.readthedocs.io/en/9.5/installation.html#requirements)

## Installation

1. **CLONEZ** ou **TÉLÉCHARGEZ** le projet
2. Ouvrez le projet dans votre IDE/éditeur de texte.
3. Configurez les variables d'environnement
Vous devez configurer au moins ces lignes dans le fichier **.env** :
``DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name?serverVersion=5.7" ``

4. Installez les dépendances avec ```composer install```.
5. Créez la base de données
Si vous êtes dans un environnement de développement, vous pouvez créer la base de données et la remplir avec du contenu factice avec la commande suivante :
```composer prepare-database```
> Alternativement, suivez les étapes suivantes :_ 
> -  Si la base de données n'existe pas, créez-la avec la commande suivante dans le répertoire du projet :
```php bin/console doctrine:database:create```.
> -  Créez la structure de la base de données grâce aux migrations :
```php bin/console doctrine:migrations:migrate```
> -  Exécutez la commande suivante pour ajouter les fixtures et obtenir du contenu factice :
```php bin/console doctrine:fixtures:load```
6. Démarrez le serveur en tapant cette ligne dans votre terminal ```php bin/console server:start```.

## Tests
##### Configuration de PHP Unit
- Si vous souhaitez modifier la configuration de PHP Unit, utilisez le fichier **phpunit.xml.dist**
- Vous devez définir DATABASE_URL pour les tests dans le fichier **env.test**. 
``` DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name_test?serverVersion=5.7" ```
- Créez la base de données de test et remplissez-la avec du contenu factice avec la commande suivante :
```composer prepare-test```
##### Exécution des tests
Pour exécuter tous les tests, utilisez la commande suivante :``make tests``

>Vous pouvez également utiliser "make help" pour voir quelles commandes "make" sont disponibles.

## Contribution

Voir le fichier [Contributing](CONTRIBUTING.md).