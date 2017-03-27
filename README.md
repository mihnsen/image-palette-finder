# image-palette-finder - A short algorithm to find the most prominent color in pictures

[Ripped from colorfinder](https://github.com/pieroxy/color-finder) :heart: @pieroxy

A short algorithm to find the most prominent color in pictures

## Usage

### Basic
``` js
new ColorFinder();
```

### Advanced
``` js
var colorfinder = new ColorFinder( function favorHue(r,g,b) {
  return (Math.abs(r-g)*Math.abs(r-g) + Math.abs(r-b)*Math.abs(r-b) + Math.abs(g-b)*Math.abs(g-b))/65535*50+1;
} );
```

### Methods

#### getImageData()
Return the image data

#### getMostProminentColor()
get the most prominent color


## Package management

Install with [Bower](http://bower.io) :bird: `bower install image-palette-finder`

Install with [npm](https://github.com/npm/npm) `npm install image-palette-finder`


## MIT license

classie is released under the [MIT license](http://www.opensource.org/licenses/mit-license.php).
