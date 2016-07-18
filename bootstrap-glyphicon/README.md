# bootstrap-glyphicon

Create a glyphicon using polymer elements. Icon value is the icon name using in bootstrap but removing `glyphicon` and `glyphicon-` style. For example: 

* glyphicon-pencil is pencil
* glyphicon-star is star
* ...

## Example

```html
<bootstrap-glyphicon icon="pencil"></bootstrap-glyphicon>
```

## Properties

| Attribute | Description                       | Type   | Default |
|-----------|-----------------------------------|--------|---------|
| __icon__    | Icon that the component will show | String | ''      |

## Custom Style

| Custom Property               | Description                          | Default |
|-------------------------------|--------------------------------------|---------|
| __--bootstrap-glyphicon-size__  | Change glyphicon size                | 12px    |
| __--bootstrap-glyphicon-style__ | Mixin applied to bootstrap-glyphicon | {}      |

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install
