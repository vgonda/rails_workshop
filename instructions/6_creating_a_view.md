## Create the view

- In `app/views/events/index.html.erb` add a loop that displays all the events

```html
<h1>Events</h1>
<table>
  <% @events.each do |event| %>
    <tr>
      <td><strong><%= event.message %></strong></td>
      <td><%= event.created_at %></td>
    </tr>
  <% end %>
</table>
```

- Run the rails server. We can see our webpage now!

```bash
rails server
```
- `Ctrl+C` stops the server