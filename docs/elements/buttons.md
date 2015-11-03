# Attributes in style

* [active](http://semantic-ui.com/elements/button.html#active)
* [disabled](http://semantic-ui.com/elements/button.html#disabled)
* [loading](http://semantic-ui.com/elements/button.html#loading)
* [size](http://semantic-ui.com/elements/button.html#size)
* [compact](http://semantic-ui.com/elements/button.html#compact)
* [fluid](http://semantic-ui.com/elements/button.html#fluid)
* [circular](http://semantic-ui.com/elements/button.html#circular)

# Colors

The attribute color can get the name you want, but there are some predefined
names.

- primary
- secondary
- danger
- info
- success

# Button

How to make a button.

You will need the basic modules and the button module.

**Attributes:**

* **text**: the button's text
* **className**: class attribute
* **color**: The color of button
* **others**: More attributes you want to add in html's tags
* **events**: The events you want to add in html's tags

**Example:**

```javascript

var React = require('react');
var ReactDOM = require('react-dom');
var button = require('semantic-ui-react/components/buttons/button');

var configButton = {
  text: 'Hello world',
  className:  ‘my-first-button’
  color: 'info',
  others: {
    id: 'hello-world-button',
    name: 'The best button'
  },
  events: {
    onClick: function(){console.log(this.props.config)}
  }
};

ReactDOM.render(React.createElement(button,{config:configButton}),document.getElementById('test'));

```

# Button Group

How to make a group of buttons.

You will need the basic modules and the buttonsGroup module.

**Attributes:**

* **group**: An array with object that contains a button and an icon
* **className**: class attribute
* **color**: The color of all butons
* **others**: More attributes you want to add in html's tags
* **icon**: A boolean to add a icon in each button
* **labeled**: A boolean to labeled the icon and button

**Example:**

```javascript

var React = require('react');
var ReactDOM = require('react-dom');
var buttonsGroup = require('semantic-ui-react/components/buttons/buttonsGroup');

var configGroupIcon = {
  group: [
    {
      button: {
        text: 'test1'
      },
      icon: {
        icon: 'Alarm'
      }
    },
    {
      button: {
        text: 'test2'
      },
      icon: {
        icon: 'Alarm'
      }
    },
  ],
  icon: true,
  style: 'vertical',
  color: 'info',
  labeled: true
};

ReactDOM.render(React.createElement(buttonsGroup,{config:configGroupIcon}),document.getElementById('test'));

```
```You can make a group with only buttons or icons```
