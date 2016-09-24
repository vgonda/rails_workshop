## Deleting an event

- Add `destroy` method to controller

```ruby
def destroy
  Event.find(params[:id]).destroy
  redirect_to events_path
end
```
- Add delete link on both the `index` and `show` pages

```ruby
<%= link_to "Delete", event_path(event), method: :delete %>
```