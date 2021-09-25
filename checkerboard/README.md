# Challenge Name

[Code Wars](https://www.codewars.com/kata/53dc08fa8a0c93229400023b/train/javascript)

## Problem

Write a method checkerboard/Checkerboard which takes an integer size and returns a checkerboard of dimensions size x size. There are two colored squares on the checkerboard. Red squares are represented by the string [r] and black squares are represented by the string [b]. You MUST use the newline character \n to insert a newline at the end of each row.

The top left corner should be a red square.
Each row should have alternating squares in the row.
The starting square on each row should also alternate.
Assumptions

You can assume you are given an integer size.
You cannot assume positive values.
Thus you should return an empty string for negative sizes and a size of 0. (An empty string does not have a newline ending).
You should assume the newline character used is \n.
You MUST leave a newline character at the end of the full checkerboard thus allowing the board to be on its own if you were to run in a terminal.

## Possible Solution

```js
// Checkerboard method
function checkerboard(size) {
  var RED = "[r]";
  var BLACK = "[b]";

  var board = "";

  for (var row = 0; row < size; row++) {
    for (var col = 0; col < size; col++) {
      board += (row + col) % 2 === 0 ? RED : BLACK;
    }
    board += "\n";
  }

  return board;
}
```
