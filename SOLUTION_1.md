# Databases - Solution Exercise #1

## SOLUTION MySQL:

    CREATE DATABASE users_db;

    CREATE TABLE users (
        id INT NOT NULL PRIMARY KEY auto_increment,
        email VARCHAR(20) NOT NULL,
        password VARCHAR(40) NULL,
        firstname VARCHAR(20) NULL,
        lastname VARCHAR(20) NULL,
        isAdmin BOOLEAN NOT NULL DEFAULT 0,
    );


## SOLUTION MongoDB:

    use users_db;
    db.createCollection("users");
