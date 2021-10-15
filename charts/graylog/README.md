

## Mongodb

Log into mongo

``bash
mongo --host localhost --username <username> --password <password>
```

Create database

```bash

```

Create user

```bash
db.createUser(
  {
    user: "graylog",
    pwd: "secret_password",
    roles: [ { role: "readWrite", db: "graylog" } ]
  }
)
```
