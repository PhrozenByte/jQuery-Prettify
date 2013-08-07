jQuery-Prettify 1.3
===================
Use google-code-prettify to highlight sourecode with jQuery

Usage
-----
Just download the sourcecode, upload the file to your webspace and load it. Obviously [jQuery](http://jquery.com/) and [google-code-prettify](https://code.google.com/p/google-code-prettify/) is required and must be loaded, too. The same applies to [jQuery-XPath](https://github.com/PhrozenByte/jQuery-XPath).
```html
<script type="text/javascript" src="js/jquery.prettify.js"></script>
```

Insert your sourcecode as follows:
```html
<div class="prettify">
  <pre>Sourecode here</pre>
</div>
```
All elements with the ```prettify``` CSS class will be prettified automatically, so you don't have to do anything. If you wan't to prettify another element (or an element you've added to the DOM later), just call ```.prettify()```.

```.prettify()``` accepts an options object as the first parameter and an callback function (same as the callback option) as second parameter. You can use HTML ```data``` attributes to set options, too (e.g. ```data-linenums="false"``` to disable line numbering). The following options are available:
* ```progress```: If you want to display a progress bar while jQuery-Prettify prettifies your sourcecode, pass a jQuery selector (e.g. ```.progress```) here.
* ```linenums```: Enable/disable line numbering (default: ```true```).
* ```auto```: Prettify the element(s) automatically when ready (default: ```true```). If you disable this, you must call ```.prettify('prettify')``` on your own.
* ```callback```: To be called function when an element has been prettified.

jQuery-Prettify has a great method to make your sourcecode more readable by expanding the sourcecode element to the width of the users browser window or as wide as necessary to prevent unwanted line breaks. You can call the following methods on the prettify element to let the box nicely grow or shrink appropriately.
* ```.prettify('viewNoLineBreak')```: Grow until no unwanted line breaks are necessary.
* ```.prettify('viewWindowWidth')```: Grow/shrink until the element is as wide as the users browser window.
* ```.prettify('viewNormal')```: Let the sourcecode appear like we've never changed its width.

License & Copyright
-------------------
Copyright (C) 2012-2013  Daniel Rudolf <http://www.daniel-rudolf.de/>

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, version 3 of the License only.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the [GNU General Public License](../blob/master/LICENSE.md) for more details.
