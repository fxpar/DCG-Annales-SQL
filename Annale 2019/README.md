# Annale 2019

## Sources
L'annale de 2019 est disponible avec son corrigé sur http://crcf.ac-grenoble.fr/index.php?tg=articles&topics=100&new=0&newc=0

## Sujet SQL

* 4. Rédigez en langage SQL (Structured Query Language) les requêtes suivantes :
  * a) Quels sont les hôtels de plein-air (nom et ville de l’hôtel) qui n’ont pas de secteur
« restauration » ?
  * b) Quel est le montant total des salaires par hôtel (numéro et nom d’hôtel) trié par ordre
alphabétique des hôtels ?
  * c) Quels sont les hôtels trois étoiles (numéro et nom de l’hôtel) qui comportent au moins
cinq secteurs ?
  * d) Suite à un changement de législation, les hôtels quatre étoiles sont reclassés en hôtel
cinq étoiles. Écrivez la requête correspondante.
  * e) Quel est le salarié (nom, prénom) qui a le salaire le plus élevé ?
  * f) Quels sont les employés (numéro, nom, prénom) de l’hôtel de plein-air « Les portes
de Bretagne » ?

M. Jean Lordino, responsable de secteur, a démissionné. La requête suivante a été préparée
pour mettre à jour la base de données.
````sql
DELETE FROM EMPLOYE
WHERE NomEmp = "Lordino"
AND PrenomEmp = "Jean"
````
  * a) À quelle condition la requête précédente peut-elle être réalisée sans message d’erreur ?
Détaillez votre réponse.

## À propos du sujet

Deux difficultés sont présentes
- la pseudo entité SECTEUR-HOTEL
- l'entité faible Appartenir-LODGE
- la contrainte d'exclusion et de totalité XT

### Saisonniers
Spontanément, j'aurais créé une table des saisonniers avec les différentes missions, d'années en années, des salariés.  
Visiblement, le créateur du sujet a eu pitié des étudiants et il me semble que ne peuvent apparaître que la "mission en cours" d'un salarié.  
Je ne pense pas que nous ayons ici la possibilité d'avoir l'historique des missions d'un même salarié saisonnier qui reviendrait. J'ai donc suivi la correction de Grenoble qui pose le champs SAISONNIER.<ins>#CodeEmp</ins> comme clé primaire
