## Setting up the database

- Create a migration

```bash
rails generate migration CreateEvent message:text
```
- Add `t.timestamps` to migration found in `db/migrations/`
- Run the migration

```bash
rake db:migrate
```
- Check out what was added to `db/schema.rb`