---
title: Js Kata One
date: 2016-11-10 15:58:36
tags: JS
---

Given a list of nested objects, each containing a single value and a reference to next object
Here is an example of a list in JavaScript:
{% codeblock %}
 {value: 1, next: { value: 2, next: { value: 3, next: null }}}
{% endcodeblock %}
Write a function that converts a list to an array, like this:

{% codeblock %}
[ 1, 2, 3 ]
{% endcodeblock %}

## Possible Answers: 

### Answer a, iterating object with for loop:
{% codeblock lang:javascript %}
function listToArray(list) {
  var arr = [];
  for ( var node = list; node; node = node.next ) {
	arr.push[node.value];
  }
  return arr;
}
{% endcodeblock %}
### Answer b, with recursion:
{% codeblock lang:javascript %}
function listToArray(list) {
  return !list ? [] : [list.value].concat(listToArray[list.next])
}
{% endcodeblock %}

from [codewars](https://www.codewars.com/kata/list-to-array/solutions).






