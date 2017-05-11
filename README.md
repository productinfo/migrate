# migrate
Command line tool for PostgreSQL migrations 

## Features

* Runs migrations in transactions
* Stores migration version details in auto-generated table ``schema_migrations``.

## Usage

```bash
migrate -url postgres://user@host:port/database -path ./db/migrations create add_field_to_table
migrate -url postgres://user@host:port/database -path ./db/migrations up
migrate -url postgres://user@host:port/database -path ./db/migrations down
migrate help # for more info
```
