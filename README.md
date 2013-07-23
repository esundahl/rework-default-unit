## rework-default-unit [![Build Status](https://travis-ci.org/fgnass/rework-default-unit.png)](https://travis-ci.org/fgnass/rework-default-unit)

[Rework](https://github.com/visionmedia/rework) plugin that adds a default unit
to numeric properties just like jQuery's `.css()` method does.

### Example

```css
.foo {
  width: 200;
  z-index: 1;
}
```

Yields:

```css
.foo {
  width: 200px;
  z-index: 1;
}
```

### Usage

```js
  var rework = require('rework');
  var defaultUnit = require('rework-default-unit');

  // Add px as default unit:
  rework(css).use(defaultUnit);

  // Add em as default unit:
  rework(css).use(defaultUnit('em'));
```

The following properties are left untouched:

* column-count
* fill-opacity
* font-weight
* line-height
* opacity
* orphans
* widows
* z-index
* zoom

### The MIT License (MIT)

Copyright (c) 2013 Felix Gnass

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
