A set of bash scripts to deal with a MariaDB database

## INSTALLATION ##

* clone repository:

`git clone https://github.com/vukbgit/mariadb-tools.git`

* setup config file:

`cp .config.template .config`

* edit config file setting:
	* db_source: name of the database to start comparison
	* db_target: name of the database to be compared to db_source
	* user: MariaDB user name into scripts
	* password: MariaDB user password
	* host and port if needed

## SCRIPTS ##

* `export.sh [database-name] [table-name]`: dumps a whole database or just a table if second argument provided

* `import.sh -d [database-name] -f [path-to-dump-file]`: imports a database from a dump file

* `create_objects.sh [object-1] [object-2] ...`: shows create sql for tables/views 
