# bootstrap-dropdown

Create a dropdown using a polymer element. It's based on boostrap dropdown.

## Example
* Using content

``` html
<bootstrap-dropdown btn_title="Content">
  <div class="menu-content">
    <p>Link 1</p>
    <p>Link 2</p>
    <p>Link 3</p>
  </div>
</bootstrap-dropdown>
```

* Using menu_items Array
```html
<template id="bind" is="dom-bind">
  <bootstrap-dropdown id="complexList" btn_title="Custom list items" menu_items="{{complexList}}"> </bootstrap-dropdown>
</template>

<script>
  var bind = document.querySelector('#bind');
  bind.complexList = [
    {
      name: 'Load',
      onclick: function(){
        console.log('Clicked Load');
      },
      link:'#load',
      icon: 'folder-open'
    },
    {
      name: 'Save',
      onclick: function(){
        console.log('Clicked Save');
      },
      link:'#option2',
      icon: 'floppy-saved'
    },
    {
      name: 'Edit',
      onclick: function(){
        console.log('Clicked Edit');
      },
      link:'#edit',
      icon: 'pencil'
    }
  ]
</script
```
NOTE: menu_items can be a single array with the names of the options fields.
```json
  var option_list = ['Link1','Link2','Link3']
```
  or it can be an object with some camps:

  * Name: name of the field
  * onclick: function which will be invoke when the field is Clicked
  * icon: type of icon


* Using bootstrap-dropdown-item (included in bootstrap-dropdown)

```html
  <bootstrap-dropdown btn_title="Toggle">
    <div class="menu-content">
      <bootstrap-dropdown-item>Example</bootstrap-dropdown-item>
      <bootstrap-dropdown-item>Example</bootstrap-dropdown-item>
      <bootstrap-dropdown-item>Example</bootstrap-dropdown-item>
    </div>
  </bootstrap-dropdown>
```

## Properties

| Attribute  | Description                                            | Type    | Default  |
|------------|--------------------------------------------------------|---------|----------|
| btn_title  | Change the button title                                | Sting   | Dropdown |
| dropup     | Menu list is showed above the button                   | Boolean | false    |
| opened     | If true, menu list is showed                           | Boolean | false    |
| menu_items | If it is defined, all items in the array are menu items | Array   | []       |


## Methods

| Attribute | Description                           | return |
|-----------|---------------------------------------|--------|
| Open      | Open menu list                        |        |
| Close     | Close menu list                       |        |
| Toggle    | If menu list, it is opened, else closed |        |

## Style

### bootstrap-dropdown

| Attribute                                        | Description                                                | Default |
|--------------------------------------------------|------------------------------------------------------------|---------|
| __--bootstrap-dropdown-btn-toggle__              | Mixin applied to bootstrap-dropdown button                 | {}      |
| __--bootstrap-dropdown-btn-toggle-focused__      | Mixin applied to bootstrap-dropdown button when is focused | {}      |
| __--bootstrap-dropdown-dropdown-box__            | Mixin aplied to menu box that contains menu options        | {}      |
| __--bootstrap-dropdown-dropdown-menuItem-hover__ | Mixin aplied to menu item when it is hovered               | {}      |
| __--bootstrap-dropdown-divider__                 | Mixin aplied to divider                                    | {}      |

### bootstrap-dropdown-item

| Attribute                                        | Description                                              | Default |
|--------------------------------------------------|----------------------------------------------------------|---------|
| __--bootstrap-dropdown-item__                    | Mixin applied to bootstrap-dropdown-item                 | {}      |
| __--bootstrap-dropdown-item-hovered__            | Mixin applied to bootstrap-dropdown-item when is focused | {}      |

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install
