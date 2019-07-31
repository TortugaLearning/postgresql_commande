demarrer en postgresql le deamon sans mot de passe

sudo -su postgres

entrer les lignes de commande en postgresql
psql

creer une base de donnees


Commande


quitter
\q

afficher les commandespsql
\h

afficher les commandes du terminal
\?

afficher la liste des roles
\du
afficher la liste des bdd
\l


Role


CREATE ROLE nom;

Permet de créer un role vierge d'ont on ne peut pas ce connecter.



CREATE USER nom;

Permet de créer un role vierge.



CREATE USER nom WITH CREATEDB;

Permet de créer un role avec l'attrubut Create DB.



CREATE USER nom WITH PASSWORD 'password';

Permet de créer un role avec un mdp.



CREATE USER nom WITH CREATEDB PASSWORD 'password';

Permet de créer un role avec l'attrubut Create DB et un mdp.



ALTER ROLE nom_role WITH CREATEDB;

Permet d'altérer le role pour lui donner l'attribut Create DB.



ALTER USER nom_role WITH PASSWORD 'password';

Permet d'altérer le role pour lui donner un mdp.



ALTER USER nom_role RENAME TO nom;

Permet d'altérer le role pour le renommer.



DROP ROLE nom_role;

Permet de supprimer le role si il n'a aucune bdd et objets.


bdd

CREATE DATABASE nom;

Permet de créer une bdd qui appartient à celui qui l'a crée.


SELECT DATABASE nom;
selectionner une database.



CREATE DATABASE nom OWNER nom_role;

Permet de créer une bdd qui appartient à nom_role.



ALTER DATABASE nom_bdd OWNER TO nom_role;

Permet d'altérer la bdd pour qu'elle appartienne à nom_role.



ALTER DATABASE nom_bdd RENAME TO nom;

Permet d'altérer la bdd pour la renommer.



DROP DATABASE nom_bdd;

Permet de supprimer la bdd et ses objets.


afficher les tables
SHOW TABLES;

renommer une table
ALTER TABLE nom_table RENAME AS nouveau_nom;

supprimer une table
DROP TABLE nom_table;


creer une table
CREATE TABLE nom_table;

mettre a jour une table

UPDATE TABLE

selectionner une table
SELECT TABLE;

rennommer une table
RENAME TABLE table1 TO table2;



ajouter une colonne 

ALTER TABLE matable ADD COLUMN macol;

AND pour ajouter une condition a WHERE
WHERE condition1 AND condition2

OR pour mettre une condition 1 ou 2
WHERE condition1 OR condition2

WHERE une condition sur sa requete
WHERE condition1 AND (condition2 OR condition3)


LIKE serta recherche les donnes qui contienne ce caractere.
SELECT * FROM table WHERE colonne LIKE modele












