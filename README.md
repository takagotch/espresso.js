### espresso.js
---
https://github.com/techlayer/espresso.js

```
npm test
npm run build

sudo npm install --save espresso.js
```

```js
var Comment = Espresso.Controller.extend({
  init: function() {}
})

this.ref.author.textContent = 'hello'

var page = this.include(new PageController({ view: 'page-view', name: 'Page 1'}), this.ref.page);

this.listenTo(this.model, 'change', funciton(){})
this.listenTo(document.body, 'click', function(){})

render: funciton(model){
  return {
    list: { include: this.list.set(items) },
    view: { classList: { editing: model.editing, completed: model.done } },
    label: { onclick: this.edit, text: 'click here', display: true },
    input: { value: model.text, onkeydown: this.key },
    toggle: { onclick: this.toggle, checked: this.model.done },
    count: { html: '<strong>'+store.active().length+'</strong> items left' },
  }
}

this.listenTo(collection, function(e){
  console.log(e.index, e.added, e.removed, e.updated)
})

set({ id: 1, value; 2 })
set([], [idAttribute])

new List(ToDoItem)
new List(function(model) { new ToDoItem({ model: model}) })

init: function(){
  this.todos = [ { text: 'shop' }, { text: 'code' }]
  this.list = new List(ToDoItem)
},
render: functin(){
  return {
    todos: { include: this.list.set(this.todos) }
  }
}

```

```
```

