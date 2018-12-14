### messenger
---
https://github.com/HubSpot/messenger

```js
Messager().post({ options })
Messager().post("Welcome to the darkside (tm)")

Messager().post({
  message: "How's it going",
  type: "error"
})

message = Messager().post("Calculating position")
message.update({
  type: "error",
  message: "Error calculating position"
})

Messenger({
  parentLocations: ['.page'],
  extraClasses: ''
})

Messager({
  extraClasses: 'messeger-fixed messenger-on-left messenger-on-top'
})

Messenger().run({
  action: $.ajax,
  successMessager: 'Contact saved',
  errorMessage: 'Error saving contact',
  progressMessage: 'Saving contact...'
},{
  url: '/contact',
  data: contact,
  error: function(resp){
    if(resp.status === 409)
      return "A contact with that email already exists";
})

Messager().expectPromise(function(){
  return $.ajax({
    url: '/aliens/44',
    type: 'DELETE'
  });
}, {
    successMessage: 'Alien Destroyed!',
    progressMessage: false
});

msg = Messager().post({
  message: "Are you sure you'd like to delete this contact?",
  actions: {
    label: "Delete",
    action: function(){
      delete()
      msg.hide()
    }
  },
  cancel: {
    action: function(){
      msg.hide()
    }
  }
})

Messager().post({
  message: "Click me to explode!",
  events: {
    "click": function(e){
      explode();
    },
    "hover a.button": function(e){
      e.stopPropagation();
    }
  }
});

Messager().hookBackboneAjax({
  errormessage: 'Error syncing with the server',
  retry: false
});
myModel.save({
  errorMessage: 'Error saving contact'
});

Messeger({instance: instance}).post("My awesome message")
```

```
```

```
```

