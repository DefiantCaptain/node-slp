# OpenSLP bindings for nodejs

[OpenSLP](http://www.openslp.org/) is an open source Service Location Protocol (SLP) implementation. You can think of SLP as a Zeroconf/Bonjour protocol.

## Installation

    npm install slp

## API

This module follows the original [OpenSLP API](http://www.openslp.org/doc/html/ProgrammersGuide/index.html) quite closely.

## Usage

Register a service

```js
var slp = require('slp');

slp.reg('service:myservice://192.168.10.1:80', slp.MAX_LIFETIME, '', function (err) {
  if (!err)
    console.log('service registered!');
});
```


## License (MIT)

The MIT License (MIT)

Copyright (c) 2013 Bug Buster Sàrl
Author: Daniel Tralamazza

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
