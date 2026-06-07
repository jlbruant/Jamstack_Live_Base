# Jamstack_Live_Base
Génération de pages statiques par une base de données / Generationg static pages from a database

Il est possible de générer des pages statiques avec une base de données.
Les bases les plus connues ont cette possibilté.

Exemple :
avec MariaDB (Mysql), il existe l' instruction OUTFILE qui permet de générer du contenu pour créer une page web rudimentaire

``select CONCAT("<div>",departement_code,"<div>") from departement into OUTFILE '/tmp/essai.html';``

Ce type de requête peut être lancée par des déclencheurs(trigger) et permettre la création du fichier de sortie au moment de l'action sur les tables de la base.

Quelle utilisation pour cette génération de pages statiques ?

- Générer des pages statiques dans une entreprise (ou une institution) avec le contenu de la base de données, en cas de panne de celle-ci ou de l'application, les données sont "sauvegardées" en temps sous forme de site intranet consultable par les utilisateurs (exemple: fournir des données patients pour assurer les soins)

Si vous avez, vous aussi utilisé cette possibilité, merci de me le faire connaitre je mettrai ici plus d'informations sur le sujet
