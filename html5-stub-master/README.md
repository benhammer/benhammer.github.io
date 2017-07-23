HTML5 Stub
==========

This repository provides a best-practices start for a new HTML5 website that supports IE8+. It was created using [Initializr](http://www.initializr.com/) with:

* H5BP 4.3.0 (with IE classes (modified), Google Analytics, Favicon, and an Apple Touch icon)
* [Boostrap 3.3.6](http://getbootstrap.com/) (Initializr is at 3.1.1, but I've updated to the latest)
* jQuery 1.11.3
* [HTML5shiv 3.6](https://github.com/aFarkas/html5shiv), which provides HTML5 support for Internet Explorer 8-9, Safari 4.x (and iPhone 3.x), and Firefox 3.x.
* [Respond.js 1.1.0](https://github.com/scottjehl/Respond#readme), which makes @media queries work in Internet Explorer 8.

The external assets listed above are loaded remotely using `https:` URLs from CDNs using subresource integrity attributes to ensure, in supported browsers, that the CDN cannot be used as an attack vector. This method is preferable in low-security environments than hosting the static resource yourself because the user will probably already have the resources in his/her cache (and why host another file?). In a high-security environment, it may be better to host everything locally to prevent a remote injection attack if the CDN is compromised.

Browser notes:

* Bootstrap only supports IE8+, but even in IE8-9 it's not perfect.
* In IE7 and earlier, the page is replaced with a note about the browser not being supported.
