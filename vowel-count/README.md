# Count Vowels

[Code Wars](https://www.codewars.com/kata/54ff3102c1bad923760001f3/train/javascript)

## Problem

Return the number (count) of vowels in the given string.

We will consider a, e, i, o, u as vowels for this Kata (but not y).

The input string will only consist of lower case letters and/or spaces.

## Possible Solution

```js
function getCount(str) {
  var vowelsCount = 0;

  for (let i = 0; i < str.length; i++) {
    if (str[i].match(/[aeiou]/)) {
      vowelsCount++;
    }
  }

  return vowelsCount;
}
```
