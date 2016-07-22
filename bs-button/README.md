# bs-button
Polymer element that use boostrap style.

[DEMO](https://mortega5.github.io/bs-button/components/bs-button/demo/)

## Example

```html
<bs-button class="success"></bs-button>
```

## Properties

| Attribute | Description                       | Type   | Default |
|-----------|-----------------------------------|--------|---------|
| __disabled__ | Disabled click on the button | Boolean | 'false'|
| __type__ | Type of the button:[Button, Submit, Reset] | String | 'button'|
| __bs_style__ | Set different style based on bootstrap button: [default, primary, info, danger, warning] | 'String' | 'default'|
| __value__ | Indicate the value of the button | String | ''|
| __size__ | Set the size of the button based on bootstrap sizes: [lg, md, sm, xm] | String |md |

### Styling

Custom property | Description | Default
----------------------|-------------|----------
|`--bs-button` | Mixin applied to the button | `{}`
|`--bs-button-active` | Mixin applied to the button when its active, focused or hovered | `{}`
|`--bs-button-disabled` | Mixin applied to the disabled button | `{}`

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Install

    bower install --save bs-button
