## Create the "new" page

- Define `event_params` in your controller

```ruby
def event_params
  params.require(:event).permit(:message)
end
```
- Define `new` and `create` in your controller

```ruby
def new
  @event = Event.new
end

def create
  Event.create(event_params)
  redirect_to events_path
end
```

- Create the form view in `app/views/events/new.html.erb`

```html
<%= form_for @event do |form| %>
  <%= form.label :message %>
  <%= form.text_field :message %>
  <%= submit_tag "Save" %>
<% end %>
```

- Add "New Event" link to `index.html.erb`

```ruby
<%= link_to "New Event", new_event_path %>
```