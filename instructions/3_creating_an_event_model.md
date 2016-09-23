## Creating an Event model

- In `app/models/event.rb` create an `Event` class that extends `ApplicationRecord`

```ruby
class Event < ApplicationRecord
end
```

- Open the rails console to interact with the class you just made

```bash
rails console
```

- Try playing around with the Ruby syntax, and the Event model.
    - `Event.new` creates an instance of `Event`
    - `Event.create` creates and saves it to the database
    - You can include attributes when you create and save: `Event.new(message: "Hello")`. You can also do this with `update`.
    - Try out some [Ruby basics](http://www.pragtob.info/rails-beginner-cheatsheet/#ruby)

    [Step 4: Creating a controller](4_creating_a_controller.md)