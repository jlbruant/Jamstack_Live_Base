# Jamstack_Live_Base
Génération de pages statiques par une base de données / Generationg static pages from a database

Il est possible de générer des pages statiques avec une base de données.
Les bases les plus connues ont cette possibilté.

Exemple :
avec MariaDB (Mysql), il existe l' instruction OUTFILE qui permet de générer du contenu pour créer une page web rudimentaire

``select CONCAT("<div>",departement_code,"<div>") from departement into OUTFILE '/tmp/essai.html';``

Le fichier html généré peut être lu par un navigateur 

Quelle utilisation pour cette génération de pages statiques ?

- Générer un intranet de secours dans une entreprise avec le contenu de la base de données en cas de panne de la base de données ou de l'application utilisant la base de données.

Si vous avez, vous aussi utilisé cette possibilité, merci de me le faire connaitre je mettrai ici plus d'informations sur le sujet
