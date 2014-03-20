# Buoy
Buoy is a simple micro-library that makes working with vanilla JS a little bit easier.

**In This Documentation**

1. [Getting Started](#getting-started)
2. [Browser Compatibility](#browser-compatibility)
3. [How to Contribute](#how-to-contribute)
4. [Changelog](#changelog)
5. [License](#license)



## Getting Started

### 1. Include Buoy on your site.

```html
<script src="js/buoy.js"></script>
```

### 2. Use Buoy in your scripts.

#### hasClass

`buoy.hasClass( element, class )` - Check if an element has a class.

```javascript
var turkey = document.querySelector('#turkey');
if ( buoy.hasClass(turkey, 'sandwich') ) {
	// Do stuff...
}
```

#### addClass

`buoy.addClass( element, class )` - Add a class to an element.

```javascript
var turkey = document.querySelector('#turkey');
buoy.addClass(turkey, 'sandwich');
```

#### removeClass

`buoy.removeClass( element, class )` - Remove a class from an element.

```javascript
var turkey = document.querySelector('#turkey');
buoy.removeClass(turkey, 'sandwich');
```

#### toggleClass

`buoy.toggleClass( element, class )` - Add or remove a class from an element.

```javascript
var turkey = document.querySelector('#turkey');
buoy.toggleClass(turkey, 'sandwich');
```

#### getSiblings

`buoy.getSiblings( element )` - Get an array of siblings for an element.

```javascript
var turkey = document.querySelector('#turkey');
var turkeyFriends = buoy.getSiblings(turkey);
Array.prototype.forEach.call(turkeyFriends, function (friends) {
	// Do stuff...
});
```

And that's it, you're done. Nice work! New to vanilla JS? Check out [Ditching jQuery for Vanilla JS](http://gomakethings.com/ditching-jquery-for-vanilla-js/).



## Browser Compatibility

Buoy works in all modern browsers, and IE 6 and above.



## How to Contribute

In lieu of a formal style guide, take care to maintain the existing coding style. Don't forget to update the version number, the changelog (in the `readme.md` file), and when applicable, the documentation.



## Changelog
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