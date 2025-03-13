# Counter Function - createCounter

## Overview
`createCounter` is a JavaScript function that creates a counter object with three operations: **increment**, **decrement**, and **reset**. It allows tracking and modifying a numerical value efficiently while maintaining state.

## Functionality
The function accepts an initial integer `init` and returns an object with three methods:

- `increment()`: Increases the current value by `1` and returns the updated value.
- `decrement()`: Decreases the current value by `1` and returns the updated value.
- `reset()`: Resets the counter to its initial value and returns it.

## Implementation
```javascript
function createCounter(init) {
  let current = init;

  return {
    increment: () => ++current,
    decrement: () => --current,
    reset: () => (current = init),
  };
}

// Example usage:
const counter = createCounter(5);
console.log(counter.increment()); // 6
console.log(counter.decrement()); // 5
console.log(counter.reset());     // 5
console.log(counter.increment()); // 6
```

## Complexity Analysis
✅ **Time Complexity:** `O(1)` for each operation, as they all execute in constant time.
✅ **Space Complexity:** `O(1)`, since only a few variables are used.

## When to Use?
- Useful for implementing simple counter logic in applications.
- Can be used for tracking button clicks, pagination counters, or user interactions.

---
🚀 **Happy Coding!**