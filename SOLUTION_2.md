# Databases - Solution Exercise #2

## Solution MySQL

    USE users_db
    
	// insert admin user

	INSERT INTO users (email, password, firstname, lastname, isAdmin)
    VALUES ('user1@web.de', "PW1", 'Firstname1', 'Lastname1', true)

	// insert two normal users

    INSERT INTO users (email, password, firstname, lastname)
    VALUES 
    ('user2@web.de', "PW2", 'Firstname2', 'Lastname2'),
    ('user3@web.de', "PW3", 'Firstname3', 'Larstname3')


## Solution MongoDB

    use users_db

    db.users.insertOne({
        email: 'user1@web.de', 
		password: "PW1", 
        firstname: 'Firstname1', 
		lastname: 'Lastname1', 
        isAdmin: true
    })

    db.users.insertMany([
        {
            email: 'user2@web.de', 
			password: "PW2", 
            firstname: 'Firstname2', 
			lastname: 'Lastname2', 
            isAdmin: false
        }, 
        {
            email: 'user3@web.de', 
			password: "PW3", 
            firstname: 'Firstname3', 
			lastname: 'Lastname3', 
            isAdmin: false
        }
    ])
