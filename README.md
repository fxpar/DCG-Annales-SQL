# DCG-Annales-SQL
Bases de données des épreuves d'annales du DCG UE8 "Système d'informations"

## Objectif
Permettre aux étudiants qui se préparent au DCG de travailler leurs requêtes en sql. 
Notamment lorsque l'université n'a pas de licence Access.

Les étudiants pourront trouver ici des bases de données sur lesquelles tester leur compétences en matière de SQL:
* requête de sélection
* requête d'ajout
* requetes de mise à jour
* requêtes de suppression


## Mode d'emploi

1. Téléchargez et installez sur votre machine le logiciel gratuit et opensource [DB Browser for Sqlite](https://sqlitebrowser.org/) disponible pour PC, Mac, Chromebook, Linux.
1. Ouvrez le dossier d'une annale (voir ci-dessus) et téléchargez le fichier se terminant par **.sqlite**
1. Dans *DB Browser for Sqlite*, cliquez sur "ouvrir une base de donnée" et choisissez le fichier de l'annale que vous venez de télécharger
1. En vous servant des différents onglet de la barre du haut, vous pouvez maintenant soit parcourir les données, soit écrire et éxécuter une requête sql
1. N'hésitez pas à cliquer dans le menu "Vue" tout en haut pour afficher le menu (DB Schéma), cela aide d'avoir la structure de la base quand on écrit sa requête
1. Le corrigé des annales est disponible en ligne sur le site de l'université de Grenoble (un grand merci aux auteurs!)

Les versions sqlite sont à utiliser avec le logiciel gratuit et opensource [DB Browser for Sqlite](https://sqlitebrowser.org/) disponible pour PC, Mac et Linux.

![Requête et structure](https://github.com/fxpar/DCG-Annales-SQL/blob/master/screenshots/2019Structure.png)

![Requête et structure](https://github.com/fxpar/DCG-Annales-SQL/blob/master/screenshots/2019RequeteEtStructure.png)



### Variante entre SQL et SQLite
La principale différence concerne les **fonctions de date** qui ne sont pas disponible en sqlite.
Pour avoir l'année d'une date on utilise la fonction strftime('%Y', maDate)

````
SELECT * from Permanent where strftime('%Y', DateEmbauche) = '2018';
````
Il n'y a pas de champs "date" en sqlite.
Le format de date utilisé ici est tout simplement un champ de type texte au format: **aaaa-mm-jj**

````
select * from Permanent where DateEmbauche BETWEEN '2015-01-01' and '2020-01-01'
````



## Ressources et détails techniques

J'ai commencé par créer les tables dans un fichier Excel.
Comme indiqué plus haut, j'ai rencontré des difficultés avec les dates, que j'ai dû convertir au format text aaaa-mm-jj.

Le logiciel de conversion https://www.rebasedata.com/convert-excel-to-sqlite-online est ensuite utilisé pour obtenir un fichier sqlite.


# Cours SQL avec Quiz intégré

https://www.fxparlant.net/decouverte-sql



