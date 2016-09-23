## Setting up the routes

- In `config/routes.rb` set the events index as the root, and create the resources routes for events

```ruby
root "events#index"
resources :events
```
- Look at the list of routes we got from this

```bash
rake routes
```

[Step 6: Creating the view](6_creating_a_view.md)