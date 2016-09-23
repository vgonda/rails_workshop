## Creating a controller
- In `app/controllers/events_controller.md` create the class `EventsController` that extends `ApplicationController`
- Create a method called `index` that gets all the events from the database, and puts them into an instance variable named `@events`

```ruby
class EventsController < ApplicationController
  def index
    @events = Event.all
  end
end
```