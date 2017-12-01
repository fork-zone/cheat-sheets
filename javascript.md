# JavaScript

## New array from existing

Return one new entry for every existing entry: `map()`

```js
const originalArray = [1, 2, 3];
const newArray = originalArray.map(item => item * 2);
console.log(newArray);
```

output:

```
[ 2, 4, 6 ]
```

## Return new array filter

Return a new array with only some of the existing entries: `filter()`

```js
const originalArray = [1, 9, 4, 2, 42]
const newArray = originalArray.filter(item => item > 5)
console.log(newArray)
```

output:

```
[ 9, 42 ]
```

## Return one new thing only

Return one new thing only: `reduce()`

```js
const originalArray = ["Alice", "Bob", "Charlie", "Bob", "Bob", "Charlie"]
const numberOfBobs = originalArray.reduce((accumulator, item) => {
  if (item === "Bob") {
    return accumulator + 1;
  } else {
    return accumulator;
  }
}, 0)
console.log(numberOfBobs)
```

output:

```
3
```