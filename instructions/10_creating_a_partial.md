## Creating a partial

- Move all duplicated code from `new.html.erb` and `edit.html.erb`, and put it in `app/views/events/_form.html.erb`
- Replace the code you removed in each file with:

```ruby
<%= render partial: “form" %>
```

[Step 11: Deleting an event](11_deleting_an_event.md)