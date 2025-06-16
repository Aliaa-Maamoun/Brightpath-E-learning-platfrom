Frontend: HTML , CSS , Javascript and Bootstrap framework.
Backend: PHP.

1)Install WAMP or XAMPP 

2)Run WAMP or XAMPP

3)Set the database:
	a/Open your browser 
	b/Type localhost/phpmyadmin/ then for the username : root 
				                  password : empty
then click on "go" 

 4)Click on "Databases", write the database name: "loginsystemtut" then click on "create"

5)Click on the "SQL" tab up top and then write this SQL code to create the first table :
  CREATE TABLE users (
idUsers int(11) AUTO_INCREMENT PRIMARY KEY NOT NULL,
uidUsers TINYTEXT NOT NULL,
emailUsers TINYTEXT NOT NULL,
pwdUsers LONGTEXT NOT NULL
);

6)Click "go" or "execute" 

7)
	a)Click on "loginsystemtut" (which is the name of our database )
	b)Click on the SQL tab up top and then write this SQL code to create the second table : 
	CREATE TABLE imgupload (
	id int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
	userid int(11) NOT NULL,
	status int(11) NOT NULL
	);

8)Click "go" or "execute" 

9)Copy the folder named "e-learning" and go inside the installation folder of  "wamp" then the folder "www" then paste.
