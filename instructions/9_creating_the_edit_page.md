## Create the "edit" page

- Define `edit` and `update` in the controller (similar to `new` and `create`)
  - Remember you can find an event with `Event.find(params[:id])`
  - You can update an event with `event.update(event_params)`
- Add link to edit on `index` and `show` pages: `edit_event_path(event)`

[Step 10: Creating a partial](10_creatin_a_partial.md)