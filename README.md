##Angular 2.X TypeScript starter kit


###Installation

Requirements:

- NodeJS

Installation:

```bash
npm install -g gulp typescript
npm install
```

To run:

```bash
gulp
```

###Usage

The starter kit is meant to be used by anyone who wants to get a taste of Angular 2.X apps 

###Install npm modules

Example:

```bash
npm install marked --save
npm install marked --save
```

###Integrate with nodeJs Project

Build should be treated as a static resource. Otherwise bundle.js is not found.

```javascript
var express = require('express');

var app = express();
app.use(express.static(__dirname + '/build'));

app.get('/', function (req, res, next) {
  res.sendFile('/build/index.html', {"root": __dirname});
});

app.listen('3002');
```

And in your html file import bundle.js as

```html
<script src="/bundle.js"></script>
```
