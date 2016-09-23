## Create the "show" page

- In your controller, create a `show` method
- Assign the event we're showing to `@event`. You can get that event with `Event.find(params[:event])`
- Create `app/views/events/show.html.erb`, and use embeded ruby to display some of the event's data
- Add link to `index.html.erb`

```ruby
<%= link_to "Show", event_path(event) %>
```