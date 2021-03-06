# 🚧 En cours d'élaboration...🚧

⚠️ il s'agit d'une version béta contenant encore des erreurs

# Objectif
 L'outil gestion des compétences de moodle permet de rattacher les compétences à des cours, et à des activités dans les cours. Il permet également de créer un plan de formation pour les étudiants.
 
 Voici une conversion du référentiel au format importable dans Moodle.
 
 ![test](https://github.com/fxpar/DCG-Annales-SQL/blob/master/R%C3%A9f%C3%A9rentiel%20Comp%C3%A9tence%20DCG%202019%20pour%20moodle/images/R%C3%A9f%C3%A9rentiel-DCG-2019-fr.png)
 
 # Version
 Il s'agit pour l'instant d'une version de travail qui contient encore de nombreuses erreur.
 
 
 # Adaptation
 
 ## Niveau
 
 Le référentiel officiel contient une hierarchies 1, 1.1, 1.1.1, ... Certains niveaux contiennent directement des compétences.
 
 Dans l'outil Moodle, on doit dire précisément si un niveau est un "domaine" ou "une compétence" (ou d'autres types: comme des valeurs...).
 (une demande de modification a été faite: [tracker](https://tracker.moodle.org/browse/MDL-70652))
 
 Nous avons donc choisi de mettre toutes les compétences dans le dernier "sous-niveau" pour obtenir un modèle clair.
 
 ## Savoirs
 Nous avons choisi de mettre les "savoirs associés" dans la Description des niveaux.
 
Le référentiel officiel 

# À Faire

* [X] Vérifier les axes
* [X] Vérifier les UE
* [X] Vérifier le niveau 1
* [X] Vérifier le niveau 2
* [ ] Vérifier le niveau 3
* [ ] Mettre les savoirs associés en liste (ul et li) au lieu de paragraphe (p)

# Ressources

## Référentiel DCG 2019
https://cache.media.enseignementsup-recherche.gouv.fr/file/25/01/5/ensup135_annexe1_1142015.pdf

## Tutoriel Moodle Compétences

Deux tuto en français pour comprendre le fonctionnement de l'outil compétences dans Moodle.

(version 2020, non répertoriée)
https://www.youtube.com/watch?v=Biwe5eXO5I8

[![Moodle Compétences 2020](https://img.youtube.com/vi/Biwe5eXO5I8/0.jpg)](https://www.youtube.com/watch?v=Biwe5eXO5I8)

(version 2017, publique)
https://www.youtube.com/watch?v=9q81Hyv0rXw

[![Moodle Compétences 2020](https://img.youtube.com/vi/9q81Hyv0rXw/0.jpg)](https://www.youtube.com/watch?v=9q81Hyv0rXw)

## Demande de modification du module compétences de moodle

* Conversation dans le forum: https://moodle.org/mod/forum/discuss.php?d=416830
* tracker https://tracker.moodle.org/browse/MDL-70652

