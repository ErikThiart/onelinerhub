# Create user with full access to single database

```sql
CREATE USER user@localhost IDENTIFIED BY 'pwd';
GRANT ALL PRIVILEGES ON db.* TO user@localhost;
FLUSH PRIVILEGES;
```

- `CREATE USER` - creates specified user
- `user@localhost` - user name and host to attach it to
- `GRANT ALL PRIVILEGES` - grants any operation for specified user
- `ON db.*` - database tables (all tables of ```db``` database in our case) we want our user to have access to
- `TO user@localhost` - user we want to grant access to (our newely created user)
- `IDENTIFIED BY 'pwd'` - set `pwd` password for our user
- `FLUSH PRIVILEGES` - will make sure new user access is granted instantly

group: create_user


link_youtube: https://youtu.be/bciXRmpiTZw
