feature: ECMAScript 5
status: use
tags: fallback gtie8 nooldmobile es5
kind: js
polyfillurls: [es5-shim](https://github.com/es-shims/es5-shim/), [augment.js](https://olivernn.github.io/augment.js/)

ECMAScript version 5 covers a large number of feature additions to what we normally call JavaScript.
Excluding IE8, [most of ES5 is supported in browsers](https://kangax.github.io/compat-table/es5/).
As it introduces no new syntax, it's possible to polyfill fairly well.
The below polyfills tackle most uses of these features, but [there is an unshimmable subset of ES5](https://gist.github.com/1664895).
Also note that some shims are known to have [edgecase compliance bugs](https://gist.github.com/1120592).
