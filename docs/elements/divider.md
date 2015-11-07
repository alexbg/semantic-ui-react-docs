# Attributes in style

* [vertical](http://semantic-ui.com/elements/divider.html#vertical-divider)
* [horizontal](http://semantic-ui.com/elements/divider.html#horizontal-divider)

# Divider

How to make a divider.

You will need the basic modules and the divider module.

**Attributes:**

* **className**: class attribute
* **others**: More attributes you want to add in html's tags
* **style**: add the semantic's class

**Example:**

```javascript

var React = require('react');
var ReactDOM = require('react-dom');
var button = require('semantic-ui-react/components/dividers/divider');

var dividerConfig = {
  className: 'divider-test',
  style: 'horizontal'
}

ReactDOM.render(React.createElement(divider,{config:dividerConfig}),document.getElementById('test'));

```
