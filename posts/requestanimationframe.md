feature: requestAnimationFrame
status: use
tags: polyfill gtie9
kind: api
polyfillurls: [requestAnimationFrame polyfill](https://gist.github.com/paulirish/1579671)

[requestAnimationFrame is recommended](http://paulirish.com/2011/requestanimationframe-for-smart-animating/) for animation as it's battery and power friendly and allows the browser to optimize the performance of your animations.

The spec has gotten some fixes and settled down. All major browsers currently support `requestAnimationFrame`. If you need full browser support, be sure to use the lightweight polyfill.

An interesting usecase: If you have vertical parallax that changes on scroll, you can consider using rAF instead of binding to a `window`'s scroll event. In this way, you'd just ask for `window.scrollTop` on your rAF callback and take action. This will give you the smoothest animations possible.
