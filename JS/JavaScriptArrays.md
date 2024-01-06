# Intrducing Arrays

`Arrays`:  
Ordered collections of values. 
- List of comments on IG post
- Collection of levels in a game
- Songs in a playlist

```javascript
let students = [];
let colors = ['red', 'orange', 'yellow'];
let lottoNums = [19, 22, 56, 12, 51];
let stuff = [true, 68, 'cat', null];
```

# Array Random Access

Arrays are indexed

|  Doc  | Dopey | Bashful | Grumpy | Sneezy | Sleepy | Happy |
| :---: | :---: | :-----: | :----: | :----: | :----: | :---: |
|   0   |   1   |    2    |   3    |   4    |   5    |   6   |
  
Each element has corressponding index (Counting starts at 0)

```javascript
let colors = ['red', 'orange', 'yellow', 'green'];

colors.length // 4

colors[0] // red
colors[0] = blue;
colors[0] // blue

colors[1] // orange
colors[2] // yellow
colors[3] // green
colors[4] // undefined
```

# Array Methods

- Push : add to end **(returns the new length of the array)**
- Pop : remove from end **(And returns it)**
- Shift : remove from start
- Unshift : add to start

More Methods
- concat : merge arrays
- includes : looks for a value
- indexOf : just like string.indexOf
- join : creates a string frmo an array
- reverse : reverses an array 
- slice : copies a portion on an array 
- splice : removes/replaces elements
- sort : sorts an array 

# Push And Pop

```javascript
let movieLine = ['tom', 'nancy'];

movieLine.push('oliver');
movieLine.push('Harry', 'Hermione');

movieLine.pop();
```

# Shift And Unshift

Shift - Removes Stuff from the start of the array.  
  
Unshift - Adds stuff at the start of an array

# Concat, indexOf, includes & reverse

Only Reverse method changes the original array (Among the given methods).   
  
It is known as `destructive`.

# Slice & Splice

## Slice 

The `slice()` method returns a shallow copy of a portion of an array into a new array object selecter from `start` to `end` (`end` not included) where `start` and `end` represent the index of items in that array . The original array will not be modified
  
`Basically substring`

## Splice

The `splice()` method changes the contents of an array by removing or replacing existing elements and/or adding new elements **in place**.

```
let arrDeleteItems = array.splice(start[, deleteCount[, item1[, item2[, ...]]]])
```

## Sort

The `sort()` method sorts the elements of an array **in place** and returns the sorted array. The default sort order is scendig, building upon converting the elements into strings, then comparing their sequesnce of UTF-16 code units values.

# Reference Types and Equality Testing


When dealing with Arrays, Javascript doesn't care about the contents, it compares their references in Memory.

# Arrays + Const

The values of the arrays can be changed as long as the reference remains the same.

# Multi-Dimentional Arrays

we can store arrays inside other arrays.