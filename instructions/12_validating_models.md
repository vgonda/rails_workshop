## Adding model validations

- Add validation to events model

```ruby
validates :message, presence: true
```
- Add check for successful save in controller's `create`

```ruby
@event = Event.new(event_params)
if @event.save
  redirect_to events_path
else
  render :new
end
```

- Add a notice in the view so the user knows if it did not save

```html
<% if @event.errors.any? %>
  <% @event.errors.full_messages.each do |message| %>
    <%= message %>
  <% end %>
<% end %>
```

- Try saving an event without a message

[Step 13: Validate on update](13_validate_on_update.md)