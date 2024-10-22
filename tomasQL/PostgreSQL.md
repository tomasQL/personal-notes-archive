
Límites de la herramienta

PostgreSQL es una herramienta dedicada al almacenamiento y tratamiento de datos. Una de las cuestiones importantes durante la elección de un sistema de administración de bases de datos es la referida al tamaño del volumen aceptado por el software. De manera general, PostgreSQL se basa extensamente en las capacidades del sistema operativo y, por lo tanto, no impone límites de volumen. Sin embargo, hay algunas excepciones:

- El tamaño de un campo está limitado a 1 gigabyte. En la práctica, este tamaño queda limitado por la cantidad de memoria RAM disponible para leer este campo.
- El tamaño de un registro está limitado a 1,6 terabytes.
- El tamaño de una tabla está limitado a 32 terabytes.
- El número máximo de columnas en una tabla puede ir desde 250 hasta 1600, según el tamaño de un bloque de datos y el tamaño de los tipos de datos utilizados para las columnas.
  
Una vez que se tienen en cuenta estas consideraciones, PostgreSQL no impone otros límites sobre el tamaño de una base de datos o la cantidad de registros en una tabla. En contraposición, el sistema operativo utilizado puede aportar sus propias limitaciones



Update Hombrew

	$ brew update
	$ brew doctor
	
Install postgreSQL

	$ brew install install postgresql@15

Starting Postgres service

	$ brew services start postgresql@15
	$ brew services list
	stop
	$ brew services stop postgreslq@15



In remote database server machine, we will need to set the PGHOST enviroment variable to the name of the database server machine as well PGPORT.

	$ psql -h localhost -p 5432 -U enzogatica -d postgres

-p Port
-U User
-d Database

Creating Databases from CLI:

	$ createdb name_db

Accesing a Database:

	$ psql name_db


Foreign Keys

[CONSTRAINT fk_name]
   FOREIGN KEY(fk_columns) 
   REFERENCES parent_table(parent_key_columns)
   [ON DELETE delete_action]
   [ON UPDATE update_action]




CloudDB for PostgreSQL

