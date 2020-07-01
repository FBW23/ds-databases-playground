# Databases - Exercise #1

## MySQL: Create a database 'users_db' with a table 'users'

Login to MySQL: `mysql -u root -p`

The table users should have the following fields:

* ID Primary Key which increases automatically
* email with max 20 characters. Nulls not allowed
* password with max 40 characters
* firstname and lastname with max 20 characters. Null allowed
* isAdmin, Boolean field with a default value of 0
	* Research how to do a boolean field in MySQL + setting a default value for a column

* Check the structure of the table afterwards using DESCRIBE

## MongoDB: Create a database 'users_db' with a collection 'users'

Login to MongoDB: `mongo`

Create the same as above. A database and a collection (=table). 

Reminder: By selecting an "empty" database "users_db" (with the USE keyword) and creating a collection "users" inside, the database will be created automatically.

Due that MongoDB is schemaless you do not need to specify any columns / ID when creating the collection. 

