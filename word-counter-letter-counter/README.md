# Count Letters and Digits

## Problem

Create a method that can determine how many letters and digits are in a given string.

Example:

```
"hel2!lo" --> 6

"wicked .. !" --> 6

"!?..A" --> 1
```

## Possible Solution

```js
function countLettersAndDigits(input) {
  return input.split("").filter((l) => l.match(/[a-z\d]/gi)).length;
}
```
