---
title: Dom Events
date: 2016-11-14 21:00:54
tags: JS
---

Given the dom structure as below:

![dom structure](/images/event-1.png  "dom structure")

Both element1 and element2 have an onClick handler, If the user click element2,  which event handler fires first?

## Two Event Models:
In the old days, Netscape and Microsoft came to different conclusions:
* Netscape said that the event on ele1 takes first. This is so called Event Capturing.
* Microsoft maintained that the event on ele2 takes precedence. This is so called Event Bubble.
### Event Capturing
![event capturing](/images/event-2.png 'event capturing')
The handler that binds on ele1 fires first, while ele2's last.
### Event Bubbling
![event bubbling](/images/event-3.png 'event bubbling')
The handler that binds on ele2 fires first, while ele1's last.
## W3C Models
In [w3c event model](https://www.w3.org/TR/DOM-Level-3-Events/#event-flow), Any event is first captured until it reaches the target element, and then bubbles up again.

![w3c event model](/images/event-4.png 'w3c event model')








