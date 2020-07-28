# DCG-Annales-SQL
Bases de données des épreuves d'annales du DCG UE8 "Système d'informations"

## Objectif
Permettre aux étudiants qui se préparent au DCG de travailler leurs requêtes en sql. 
Les étudiants pourront trouver ici des bases de données sur lesquels tester leur compétences en matière de SQL

## Fonctionnement

### Logiciel recommandés
Les versions sqlite sont à utiliser avec le logiciel "DB Browser for Sqlite" disponible pour PC, Mac et Linux.

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
