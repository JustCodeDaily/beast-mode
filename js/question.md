# Day 1: JavaScript Type Coercion

## Difficulty
Beginner

## Topic
Type Coercion in JavaScript

## Objective
Understand how JavaScript coerces types implicitly and recognize common pitfalls.

---

## Task Description

JavaScript automatically converts values between types in certain operations. This behavior is called **type coercion**. Predict the output and explain the *why* behind each result.

---

## Code Snippet

```javascript
console.log("5" + 3);
console.log("5" - 3);
console.log(null == undefined);
console.log(null === undefined);
```

---

## Requirements

1. **Predict the output** of each line.
2. **Explain the reason** for each output (1-2 lines max).
3. **Identify when this bites you** in real code (give one practical example).
4. **Bonus:** Explain the difference between `==` and `===`.

---

## Deliverable

Provide your answer in this format:

```
Output 1: [your answer]
Reason: [explanation]

Output 2: [your answer]
Reason: [explanation]

Output 3: [your answer]
Reason: [explanation]

Output 4: [your answer]
Reason: [explanation]

Real-world gotcha: [practical example]

Bonus: [== vs === explanation]
```

---

## Hints

- Think about what the `+` operator does with strings.
- The `-` operator doesn't concatenate—it coerces to numbers.
- `==` is loose equality; `===` is strict equality.
