# Databases - Solution Exercise #3

## Solution MySQL

#1 Filter for NON admins

`SELECT * FROM users WHERE isAdmin = 0`

#2 Update user 3 password to "NEW_PW" (pick him by email)

`UPDATE users SET password = "NEW_PW" WHERE email = "user3@web.de"`

#3 Delete user 3 by ID

```
DELETE FROM users WHERE id = 3
```

## Solution MongoDB

#1 Filter for NON admins

`db.users.find({isAdmin: false})`

#2 Update user 3 password to "NEW_PW" by email

`db.users.findOneAndUpdate({email: "user3@web.de"}, {$set: {password: "NEW_PW"}})`

#3 Delete user 3 by ID

```
db.users.findOneAndDelete({_id: ObjectId("<yourIdOfUser3>")})
```

