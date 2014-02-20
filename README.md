*This repository is a mirror of the [component](http://component.io) module [pazguille/editable](http://github.com/pazguille/editable). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/pazguille-editable`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# Editable Component

  Simple and tiny Edit in place for component

## Installation

    $ component install pazguille/editable

## API

### Configuration
- `title` Text for title

### Events
- `done` It's emitted when set a new content
- `cancel` It's emitted when cancel the edit

## Example
### HTML
```
<div id="example">Everything contained within this div is editable.</div>
```

### JavaScript
```javascript
// Creates a new editable component
var Editable = require('editable');
var element = document.getElementById('example');
var edit = new Editable(element, 'Please, edit it!');

// Binds events
edit.on('done', function (event, data) {
	// Some code here!
	// For example, you can send data to the server by ajax,
	// or save into localStorage.
	// Parameter 'data' is the current content.
});

edit.on('cancel', function (event, data) {
	// Some code here!
});
```

## Contact
- Guille Paz (Frontend developer - JavaScript developer | Web standards lover)
- E-mail: [guille87paz@gmail.com](mailto:guille87paz@gmail.com)
- Twitter: [@pazguille](http://twitter.com/pazguille)
- Web: [http://pazguille.me](http://pazguille.me)

## License
### The MIT License
Copyright (c) 2012 [@pazguille](http://twitter.com/pazguille)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.