## Adding attributes

- Create a migration to add relevance to event

```bash
rails generate migration AddRelevanceToEvent relevance:integer
```

- Add a default value by appending the column creation in the migration

```ruby
default: 0
```
- Run the migration

```bash
rake db:migrate
```
- Add the attribute to the `event_params`

```ruby
params.require(:event).permit(:message, :relevence)
```

- Add the attribute on all the fields
  - You can use `form.number_field` in the form

