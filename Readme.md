<h1 align="center">cheerio</h1>

# Modified
- Updated htmlparser2 
- Removed parse5 module (around 50% of total bundle size)
- Browserified and minified: `npm run bundle` (browserify and terser required) => now only 185KB
- Improved load performance: 2x-5x faster vs. parse5

<h5 align="center">Fast, flexible & lean implementation of core jQuery designed specifically for the server.</h5>

<div align="center">
  <a href="http://travis-ci.org/cheeriojs/cheerio">
    <img src="https://secure.travis-ci.org/cheeriojs/cheerio.svg?branch=master" alt="Travis CI" />
  </a>
  <a href="https://coveralls.io/r/cheeriojs/cheerio">
    <img src="http://img.shields.io/coveralls/cheeriojs/cheerio.svg?branch=master&style=flat" alt="Coverage" />
  </a>
  <a href="https://gitter.im/cheeriojs/cheerio?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge">
    <img src="https://badges.gitter.im/Join%20Chat.svg" alt="Join the chat at https://gitter.im/cheeriojs/cheerio" />
  </a>
  <a href="#backers">
    <img src="https://opencollective.com/cheerio/backers/badge.svg" alt="OpenCollective backers"/>
  </a>
  <a href="#sponsors">
    <img src="https://opencollective.com/cheerio/sponsors/badge.svg" alt="OpenCollective sponsors"/>
  </a>
</div>

<br />

```js
const cheerio = require('cheerio')
const $ = cheerio.load('<h2 class="title">Hello world</h2>')

$('h2.title').text('Hello there!')
$('h2').addClass('welcome')

$.html()
//=> <html><head></head><body><h2 class="title welcome">Hello there!</h2></body></html>
```

## Installation
`npm install cheerio`

## Features
__&#10084; Familiar syntax:__
Cheerio implements a subset of core jQuery. Cheerio removes all the DOM inconsistencies and browser cruft from the jQuery library, revealing its truly gorgeous API.

__&#991; Blazingly fast:__
Cheerio works with a very simple, consistent DOM model. As a result parsing, manipulating, and rendering are incredibly efficient. Preliminary end-to-end benchmarks suggest that cheerio is about __8x__ faster than JSDOM.

__&#10049; Incredibly flexible:__
Cheerio wraps around [parse5](https://github.com/inikulin/parse5) parser and can optionally use @FB55's forgiving [htmlparser2](https://github.com/fb55/htmlparser2/). Cheerio can parse nearly any HTML or XML document.

## Cheerio is not a web browser

Cheerio parses markup and provides an API for traversing/manipulating the resulting data structure. It does not interpret the result as a web browser does. Specifically, it does *not* produce a visual rendering, apply CSS, load external resources, or execute JavaScript. If your use case requires any of this functionality, you should consider projects like [PhantomJS](http://phantomjs.org/) or [JSDom](https://github.com/tmpvar/jsdom).

## Sponsors

Does your company use Cheerio in production? Please consider [sponsoring this project](https://opencollective.com/cheerio#sponsor). Your help will allow maintainers to dedicate more time and resources to its development and support.

<a href="https://opencollective.com/cheerio/sponsor/0/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/0/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/1/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/1/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/2/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/2/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/3/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/3/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/4/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/4/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/5/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/5/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/6/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/6/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/7/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/7/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/8/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/8/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/9/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/9/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/10/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/10/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/11/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/11/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/12/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/12/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/13/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/13/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/14/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/14/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/15/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/15/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/16/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/16/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/17/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/17/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/18/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/18/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/19/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/19/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/20/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/20/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/21/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/21/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/22/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/22/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/23/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/23/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/24/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/24/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/25/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/25/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/26/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/26/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/27/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/27/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/28/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/28/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/sponsor/29/website" target="_blank"><img src="https://opencollective.com/cheerio/sponsor/29/avatar.svg"></a>

## Backers

[Become a backer](https://opencollective.com/cheerio#backer) to show your support for Cheerio and help us maintain and improve this open source project.

<a href="https://opencollective.com/cheerio/backer/0/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/0/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/1/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/1/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/2/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/2/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/3/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/3/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/4/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/4/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/5/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/5/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/6/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/6/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/7/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/7/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/8/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/8/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/9/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/9/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/10/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/10/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/11/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/11/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/12/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/12/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/13/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/13/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/14/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/14/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/15/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/15/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/16/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/16/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/17/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/17/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/18/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/18/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/19/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/19/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/20/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/20/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/21/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/21/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/22/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/22/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/23/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/23/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/24/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/24/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/25/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/25/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/26/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/26/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/27/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/27/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/28/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/28/avatar.svg"></a>
<a href="https://opencollective.com/cheerio/backer/29/website" target="_blank"><img src="https://opencollective.com/cheerio/backer/29/avatar.svg"></a>

## API

### Markup example we'll be using:

```html
<ul id="fruits">
  <li class="apple">Apple</li>
  <li class="orange">Orange</li>
  <li class="pear">Pear</li>
</ul>
```

This is the HTML markup we will be using in all of the API examples.

### Loading
First you need to load in the HTML. This step in jQuery is implicit, since jQuery operates on the one, baked-in DOM. With Cheerio, we need to pass in the HTML document.

This is the _preferred_ method:

```js
const cheerio = require('cheerio');
const $ = cheerio.load('<ul id="fruits">...</ul>');
```

Optionally, you can also load in the HTML by passing the string as the context:

```js
const $ = require('cheerio');
$('ul', '<ul id="fruits">...</ul>');
```

Or as the root:

```js
const $ = require('cheerio');
$('li', 'ul', '<ul id="fruits">...</ul>');
```

If you need to modify parsing options for XML input, you may pass an extra
object to `.load()`:

```js
const $ = cheerio.load('<ul id="fruits">...</ul>', {
    xml: {
      normalizeWhitespace: true,
    }
});
```

The options in the `xml` object are taken directly from [htmlparser2](https://github.com/fb55/htmlparser2/wiki/Parser-options), therefore any options that can be used in `htmlparser2` are valid in cheerio as well. The default options are:

```js
{
    withDomLvl1: true,
    normalizeWhitespace: false,
    xmlMode: true,
    decodeEntities: true
}
```

For a full list of options and their effects, see [this](https://github.com/fb55/DomHandler) and
[htmlparser2's options](https://github.com/fb55/htmlparser2/wiki/Parser-options).

Some users may wish to parse markup with the `htmlparser2` library, and
traverse/manipulate the resulting structure with Cheerio. This may be the case
for those upgrading from pre-1.0 releases of Cheerio (which relied on
`htmlparser2`), for those dealing with invalid markup (because `htmlparser2` is
more forgiving), or for those operating in performance-critical situations
(because `htmlparser2` may be faster in some cases). Note that "more forgiving"
means `htmlparser2` has error-correcting mechanisms that aren't always a match
for the standards observed by web browsers. This behavior may be useful when
parsing non-HTML content.

To support these cases, `load` also accepts a `htmlparser2`-compatible data
structure as its first argument. Users may install `htmlparser2`, use it to
parse input, and pass the result to `load`:

```js
// Usage as of htmlparser2 version 3:
const htmlparser2 = require('htmlparser2');
const dom = htmlparser2.parseDOM(document, options);

const $ = cheerio.load(dom);
```

### Selectors

Cheerio's selector implementation is nearly identical to jQuery's, so the API is very similar.

#### $( selector, [context], [root] )
`selector` searches within the `context` scope which searches within the `root` scope. `selector` and `context` can be a string expression, DOM Element, array of DOM elements, or cheerio object. `root` is typically the HTML document string.

This selector method is the starting point for traversing and manipulating the document. Like jQuery, it's the primary method for selecting elements in the document, but unlike jQuery it's built on top of the CSSSelect library, which implements most of the Sizzle selectors.

```js
$('.apple', '#fruits').text()
//=> Apple

$('ul .pear').attr('class')
//=> pear

$('li[class=orange]').html()
//=> Orange
```

##### XML Namespaces
You can select with XML Namespaces but [due to the CSS specification](https://www.w3.org/TR/2011/REC-css3-selectors-20110929/#attribute-selectors), the colon (`:`) needs to be escaped for the selector to be valid.

```js
$('[xml\\:id="main"');
```

### Rendering
When you're ready to render the document, you can call the `html` method on the "root" selection:

```js
$.root().html()
//=>  <html>
//      <head></head>
//      <body>
//        <ul id="fruits">
//          <li class="apple">Apple</li>
//          <li class="orange">Orange</li>
//          <li class="pear">Pear</li>
//        </ul>
//      </body>
//    </html>
```

If you want to render the [`outerHTML`](https://developer.mozilla.org/en-US/docs/Web/API/Element/outerHTML) of a selection, you can use the `html` utility functon:

```js
cheerio.html($('.pear'))
//=> <li class="pear">Pear</li>
```

By default, `html` will leave some tags open. Sometimes you may instead want to render a valid XML document. For example, you might parse the following XML snippet:

```xml
const $ = cheerio.load('<media:thumbnail url="http://www.foo.com/keyframe.jpg" width="75" height="50" time="12:05:01.123"/>');
```

... and later want to render to XML. To do this, you can use the 'xml' utility function:

```js
$.xml()
//=>  <media:thumbnail url="http://www.foo.com/keyframe.jpg" width="75" height="50" time="12:05:01.123"/>
```

You may also render the text content of a Cheerio object using the `text` static method:

```js
const $ = cheerio.load('This is <em>content</em>.')
cheerio.text($('body'))
//=> This is content.
```

### Plugins

Once you have loaded a document, you may extend the prototype or the equivalent `fn` property with custom plugin methods:

```js
const $ = cheerio.load('<html><body>Hello, <b>world</b>!</body></html>');
$.prototype.logHtml = function() {
  console.log(this.html());
};

$('body').logHtml(); // logs "Hello, <b>world</b>!" to the console
```

### The "DOM Node" object

Cheerio collections are made up of objects that bear some resemblence to [browser-based DOM nodes](https://developer.mozilla.org/en-US/docs/Web/API/Node). You can expect them to define the following properties:

- `tagName`
- `parentNode`
- `previousSibling`
- `nextSibling`
- `nodeValue`
- `firstChild`
- `childNodes`
- `lastChild`

## Screencasts

http://vimeo.com/31950192

> This video tutorial is a follow-up to Nettut's "How to Scrape Web Pages with Node.js and jQuery", using cheerio instead of JSDOM + jQuery. This video shows how easy it is to use cheerio and how much faster cheerio is than JSDOM + jQuery.

## Contributors

These are some of the contributors that have made cheerio possible:

```
project  : cheerio
 repo age : 2 years, 6 months
 active   : 285 days
 commits  : 762
 files    : 36
 authors  :
   293  Matt Mueller            38.5%
   133  Matthew Mueller         17.5%
    92  Mike Pennisi            12.1%
    54  David Chambers          7.1%
    30  kpdecker                3.9%
    19  Felix Böhm             2.5%
    17  fb55                    2.2%
    15  Siddharth Mahendraker   2.0%
    11  Adam Bretz              1.4%
     8  Nazar Leush             1.0%
     7  ironchefpython          0.9%
     6  Jarno Leppänen         0.8%
     5  Ben Sheldon             0.7%
     5  Jos Shepherd            0.7%
     5  Ryan Schmukler          0.7%
     5  Steven Vachon           0.7%
     4  Maciej Adwent           0.5%
     4  Amir Abu Shareb         0.5%
     3  jeremy.dentel@brandingbrand.com 0.4%
     3  Andi Neck               0.4%
     2  steve                   0.3%
     2  alexbardas              0.3%
     2  finspin                 0.3%
     2  Ali Farhadi             0.3%
     2  Chris Khoo              0.3%
     2  Rob Ashton              0.3%
     2  Thomas Heymann          0.3%
     2  Jaro Spisak             0.3%
     2  Dan Dascalescu          0.3%
     2  Torstein Thune          0.3%
     2  Wayne Larsen            0.3%
     1  Timm Preetz             0.1%
     1  Xavi                    0.1%
     1  Alex Shaindlin          0.1%
     1  mattym                  0.1%
     1  Felix Böhm            0.1%
     1  Farid Neshat            0.1%
     1  Dmitry Mazuro           0.1%
     1  Jeremy Hubble           0.1%
     1  nevermind               0.1%
     1  Manuel Alabor           0.1%
     1  Matt Liegey             0.1%
     1  Chris O'Hara            0.1%
     1  Michael Holroyd         0.1%
     1  Michiel De Mey          0.1%
     1  Ben Atkin               0.1%
     1  Rich Trott              0.1%
     1  Rob "Hurricane" Ashton  0.1%
     1  Robin Gloster           0.1%
     1  Simon Boudrias          0.1%
     1  Sindre Sorhus           0.1%
     1  xiaohwan                0.1%
```

## Cheerio in the real world

Are you using cheerio in production? Add it to the [wiki](https://github.com/cheeriojs/cheerio/wiki/Cheerio-in-Production)!

## Testing

To run the test suite, download the repository, then within the cheerio directory, run:

```shell
make setup
make test
```

This will download the development packages and run the test suite.

## Special Thanks

This library stands on the shoulders of some incredible developers. A special thanks to:

__&#8226; @FB55 for node-htmlparser2 & CSSSelect:__
Felix has a knack for writing speedy parsing engines. He completely re-wrote both @tautologistic's `node-htmlparser` and @harry's `node-soupselect` from the ground up, making both of them much faster and more flexible. Cheerio would not be possible without his foundational work

__&#8226; @jQuery team for jQuery:__
The core API is the best of its class and despite dealing with all the browser inconsistencies the code base is extremely clean and easy to follow. Much of cheerio's implementation and documentation is from jQuery. Thanks guys.

__&#8226; @visionmedia:__
The style, the structure, the open-source"-ness" of this library comes from studying TJ's style and using many of his libraries. This dude consistently pumps out high-quality libraries and has always been more than willing to help or answer questions. You rock TJ.

## License

MIT
