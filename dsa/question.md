# Day 1: DSA—Array Indexing & Edge Cases

## Difficulty
Beginner

## Topic
Arrays, Indexing, and Boundary Handling

## Objective
Understand zero-based indexing and write defensive code to handle out-of-bounds access.

---

## Task Description

Arrays in JavaScript (and most languages) use zero-based indexing. Write a function that safely retrieves elements and finds indices, handling edge cases gracefully.

---

## Scenarios

```
Array: [10, 20, 30, 40, 50]

1. Find the element at index 2.
2. Find the index of element 40.
3. What happens if you access index 10?
```

---

## Requirements

1. **Answer the three scenarios** (1 line each).
2. **Write a function `getElement(arr, index)`** that:
   - Returns the element at the given index (if valid).
   - Returns `null` or an error message if index is out of bounds.
   - Handles negative indices gracefully (optional).
3. **Write a function `findIndex(arr, value)`** that:
   - Returns the index of the first occurrence of `value`.
   - Returns `-1` if the value is not found.
4. **Provide test cases** for both functions.

---

## Deliverable

Provide your answer in this format:

```markdown
## Scenario Answers

1. Element at index 2: [answer]
2. Index of 40: [answer]
3. Accessing index 10: [answer]

## Code Solutions

### getElement Function
[paste your function]

### findIndex Function
[paste your function]

## Test Cases
[show at least 3 test cases for each function]
```

---

## Hints

- Arrays in JavaScript are 0-indexed: `arr[0]` is the first element.
- Out-of-bounds access returns `undefined`.
- Use `.indexOf()` or `.findIndex()` to search, or implement manually.
- Always check array length before accessing by index.
