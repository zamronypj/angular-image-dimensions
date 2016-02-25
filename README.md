angular-image-dimensions
------------------

Angular directive for getting and display displaying image dimensions in the view.

Installation
------------

Install via npm:

```
npm install angular-image-dimensions
```

Install via bower:

```
bower install angular-image-dimensions
```

Getting Started
---------------

If using CommonJS:

```
var ngImageDimensions = require('ngImageDimensions');
```

If using AMD:

```
require(['ngImageDimensions'], function () {});
```

If using normal browser include:

```
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.9/angular.min.js", type="text/javascript"></script>
<script src="angular-image-dimensions.js" type="text/javascript"></script>
```

Usage
-----

Once the module has been included into your project, just add it to your angular application.

```
angular.module('myApp', ['ngImageDimensions'])
```

Include the directive onto an element that contains an image.

```
<div image-dimensions>
    <img src="image.jpg" alt="image" title="image" />
    <span>{{ dimensions }}</span>
</div>
```

The directive will query the browser for the image dimensions and then will output them into the view on a scope variable named dimensions.

Compatibility
-------------

This plugin utilizes the HTML5 spec of `naturalWidth` and `naturalHeight`, therefore is only supported in browsers that support HTML5.


License (MIT)
-------------

angular-image-dimensions is distributed under the MIT License:

```
Copyright (c) 2016 Scott Lanning

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```