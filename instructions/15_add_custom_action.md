## Adding custom actions

- Add a member action on the resources route

```ruby
resources :events do
  member do
    get :add_relevance
  end
end
```
- See what route was added

```bash
rake routes
```
- Create a `add_relevance` method to the controller

```ruby
def add_relevance
  @event = Event.find(params[:id])
  @event.relevence += 1
  @event.save
  redirect_to event_path(@event)
end
```
- Add link to perform action: `add_relevance_event_path(@event)`

- Now do the same to decrement relevance