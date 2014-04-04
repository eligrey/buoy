# Buoy
Buoy is a simple `classList` polyfill that makes working with classes in vanilla JS a little bit easier.

**In This Documentation**

1. [Getting Started](#getting-started)
2. [Browser Compatibility](#browser-compatibility)
3. [How to Contribute](#how-to-contribute)
4. [Changelog](#changelog)
5. [License](#license)
6. [Older Docs](#older-docs)



## Getting Started

### 1. Include Buoy on your site.

```html
<script src="js/buoy.js"></script>
```

### 2. Use `classList` as normal in your scripts.

#### contains

`element.classList.contains( class )` - Check if an element has a class.

```javascript
var sandwich = document.querySelector('#sandwich');
if ( sandwich.classList.contains( 'turkey' ) ) {
	// Do stuff...
}
```

#### add

`element.classList.add( class )` - Add a class to an element.

```javascript
var sandwich = document.querySelector('#sandwich');
sandwich.classList.add( 'turkey' );
```

#### remove

`element.classList.remove( class )` - Remove a class from an element.

```javascript
var sandwich = document.querySelector('#sandwich');
sandwich.classList.remove( 'turkey' );
```

#### toggle

`element.classList.remove( class )` - Add or remove a class from an element.

```javascript
var sandwich = document.querySelector('#sandwich');
sandwich.classList.toggle( 'turkey' );
```

And that's it, you're done. Nice work! New to vanilla JS? Check out [Ditching jQuery for Vanilla JS](http://gomakethings.com/ditching-jquery-for-vanilla-js/).



## Browser Compatibility

Buoy extends vanilla JavaScript `classList` support back to IE 8 and above.



## How to Contribute

In lieu of a formal style guide, take care to maintain the existing coding style. Don't forget to update the version number, the changelog (in the `readme.md` file), and when applicable, the documentation.



## Changelog

* v2.0 - April 4, 2013
	* Converted from dedicated methods to `classList` polyfill. Promotes future-friendly coding, and allows you easily remove Buoy from projects when `classList` support is more widespread.
	* Removed `getSiblings` method, which was rarely used.
* v1.2 - November 10, 2013
	* Updated regex patterns.
	* Added `classList` function for supporting browsers.
	* Both updates adapted from [Apollo by Todd Motto](https://github.com/toddmotto/apollo).
* v1.1 - August 27, 2013
	* Added missing semicolons.
	* Activated strict mode.
* v1.0 - August 26, 2013
	* Initial release.



## License

Buoy is licensed under the [MIT License](http://gomakethings.com/mit/).



## Older Docs

* [Version 1](https://github.com/cferdinandi/buoy/tree/archive-v1)