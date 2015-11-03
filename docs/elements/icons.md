# Attributes in style

* [fitted](http://semantic-ui.com/elements/button.html#fitted)
* [disabled](http://semantic-ui.com/elements/button.html#disabled)
* [loading](http://semantic-ui.com/elements/button.html#loading)
* [size](http://semantic-ui.com/elements/button.html#size)
* [circular](http://semantic-ui.com/elements/button.html#circular)
* [bordered](http://semantic-ui.com/elements/button.html#bordered)
* [link](http://semantic-ui.com/elements/button.html#link)
* [rotated](http://semantic-ui.com/elements/button.html#rotated)

# Colors

The attribute color can get the name you want, but there are some predefined
names.

- primary
- secondary
- danger
- info
- success

# Icon

How to make a icon.

You will need the basic modules and the icon module.

**Attributes:**

* **text**: the button's text
* **className**: class attribute
* **color**: The color of icon
* **others**: More attributes you want to add in html's tags
* **events**: The events you want to add in html's tags

**Example:**

```javascript

var React = require('react');
var ReactDOM = require('react-dom');
var icon = require('semantic-ui-react/components/icons/icon');

var iconConfig = {
  className: 'icon-test',
  icon: 'Alarm',
  style: 'circular',
  color: 'danger'
}

ReactDOM.render(React.createElement(icon,{config:iconConfig}),document.getElementById('test'));

```
