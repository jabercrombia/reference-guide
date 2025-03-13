# JavaScript Higher-Order Functions: Map, Reduce, Filter, and More

## Overview
This document provides an overview of essential JavaScript higher-order functions used for array manipulation: `map`, `reduce`, `filter`, and additional functions such as `forEach`, `find`, and `some/every`.

## 1. map()
The `map` method creates a new array by applying a function to each element of the original array.

### Syntax:
```javascript
const newArray = array.map(callback(element, index, array));
```

### Example:
```javascript
const numbers = [1, 2, 3, 4];
const squared = numbers.map(num => num * num);
console.log(squared); // [1, 4, 9, 16]
```

## 2. reduce()
The `reduce` method reduces an array to a single value by executing a reducer function on each element.

### Syntax:
```javascript
const result = array.reduce((accumulator, element, index, array) => { /* logic */ }, initialValue);
```

### Example:
```javascript
const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((acc, num) => acc + num, 0);
console.log(sum); // 10
```

## 3. filter()
The `filter` method creates a new array with elements that pass a test specified by the provided function.

### Syntax:
```javascript
const newArray = array.filter(callback(element, index, array));
```

### Example:
```javascript
const numbers = [1, 2, 3, 4, 5, 6];
const evenNumbers = numbers.filter(num => num % 2 === 0);
console.log(evenNumbers); // [2, 4, 6]
```

## 4. forEach()
The `forEach` method executes a function once per array element but does not return a new array.

### Syntax:
```javascript
array.forEach(callback(element, index, array));
```

### Example:
```javascript
const numbers = [1, 2, 3];
numbers.forEach(num => console.log(num * 2));
// Output: 2, 4, 6
```

## 5. find()
The `find` method returns the first element that satisfies the given condition.

### Syntax:
```javascript
const result = array.find(callback(element, index, array));
```

### Example:
```javascript
const numbers = [1, 2, 3, 4];
const firstEven = numbers.find(num => num % 2 === 0);
console.log(firstEven); // 2
```

## 6. some() and every()
- `some()`: Returns `true` if at least one element satisfies the condition.
- `every()`: Returns `true` only if all elements satisfy the condition.

### Syntax:
```javascript
const hasCondition = array.some(callback(element, index, array));
const allCondition = array.every(callback(element, index, array));
```

### Example:
```javascript
const numbers = [2, 4, 6];
console.log(numbers.some(num => num % 2 !== 0)); // false (no odd numbers)
console.log(numbers.every(num => num % 2 === 0)); // true (all even numbers)
```

## Conclusion
These higher-order functions provide efficient and readable ways to manipulate arrays in JavaScript. Use them to simplify operations and avoid unnecessary loops.

