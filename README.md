# timeago-es

A wrapper for Ryan McGeary's [jQuery plugin](http://timeago.yarp.com/) (Spanish translation).

![timeago](http://i.imgur.com/W1Zwy.png)

#install

    npm install timeago-es

#usage

````javascript
var timeago = require('timeago-es');

var pretty = timeago(+new Date());

console.log(pretty); // just now
````

You can also use it in Express app templates:

````javascript
var app = express.createServer();

app.helpers({
  timeago: require('timeago-es')
});
````

````ejs
<div class="timeago"><%- timeago(widget.created) %></div>
````
