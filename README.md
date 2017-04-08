# Generate Dynamic sitemap from a MySQL database from PHP

Need to generate a sitemap.xml to submit to Google for your Dynamic PHP+MYSQL Sites?

Have pages like /Info/something-from-db ?

Ex: http://gurupaara.lk/Teacher/sanjeewa-dharmawardhana **sanjeewa-dharmawardhana** this part from DB. 


Simply change the configuration and generate it.

```PHP
// CONFIGURATION
	// Set a password to limit access to generating XML's
	$token = "mypassword";
	// Set your MySQL details 
	$servername="localhost";
	$username="USER";
	$password="PASS";
	$dbname="DBNAME";
	// Set your custom table name to generate 
	$table_name  = "TABLE_NAME";
	// Set your custom column name to generate 
	$column_name  = "COLUMN_NAME";
	// Your site Base URL
	$base_url = "http://gurupaara.lk/";
	$frequency = "weekly";
	// These are the static/page/subdirectories you need to include in the site map
	$static_pages = array("","index.php","forum/","about.php", "Institutes.php", "contact.php", "environment.php","blog/");
	
// END CONFIGURATION

```
