# sequelize-ts-model-generator
Generate Sequelize model and migrations in typescript

## Description
Il s'agit d'un extrait de code Node.js permettant de générer un modèle Sequelize et un fichier de migration pour une table de base de données. Le code utilise la bibliothèque pluralize pour générer les noms de table au pluriel et la bibliothèque yargs pour analyser les arguments en ligne de commande. Les fichiers de modèle et de migration générés sont écrits dans des répertoires distincts pour les modèles et les migrations, au format TypeScript.

## Dépendances
Les dépendances suivantes sont nécessaires pour exécuter ce code :

- Node.js
- La bibliothèque pluralize
- La bibliothèque yargs
- Le module fs (intégré à Node.js)

## Installation
Pour installer les dépendances requises, exécutez la commande suivante :

    npm install pluralize yargs

## Utilisation
Incluez les bibliothèques pluralize et yargs en haut de votre fichier :

    const pluralize = require('pluralize');
    const args = require('yargs').argv;

Définissez les variables et fonctions nécessaires pour votre utilisation spécifique. Le code fourni dans cet extrait est un exemple générique.
Appelez la fonction modelTSConstructor() pour générer le modèle et la migration en utilisant les arguments appropriés. Assurez-vous de fournir les attributs nécessaires sous forme d'arguments en ligne de commande, par exemple :

    node script.js --name MyModel --attributes attr1:string,attr2:integer,attr3:date

Cela générera un modèle Sequelize et un fichier de migration pour une table de base de données avec le nom "MyModel" et les attributs spécifiés. Les fichiers générés seront écrits dans les répertoires appropriés et seront prêts à être utilisés dans votre application.

## Avertissement
Assurez-vous de bien comprendre le code avant de l'utiliser dans votre application, et de le personnaliser en fonction de vos besoins spécifiques. Ce code est fourni à titre d'exemple et peut nécessiter des modifications pour s'adapter à votre environnement de développement et à vos besoins particuliers.