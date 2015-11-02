# Attributes in type

* [active](http://semantic-ui.com/elements/button.html#active)
* [disabled](http://semantic-ui.com/elements/button.html#disabled)
* [loading](http://semantic-ui.com/elements/button.html#loading)
* [size](http://semantic-ui.com/elements/button.html#size)
* [compact](http://semantic-ui.com/elements/button.html#compact)
* [fluid](http://semantic-ui.com/elements/button.html#fluid)
* [circular](http://semantic-ui.com/elements/button.html#circular)


# Button

How to make a button.

You will need the basic module and the button module.

```javascript

var React = require('react');
var ReactDOM = require('react-dom');
var button = require('button');

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
