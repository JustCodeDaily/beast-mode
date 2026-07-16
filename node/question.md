# Day 1: Node.js Event Loop—Sync vs Async

## Difficulty
Beginner

## Topic
Event Loop, Macrotasks, Microtasks, and Execution Order

## Objective
Understand JavaScript's event loop and why Promise callbacks execute before setTimeout callbacks.

---

## Task Description

JavaScript has a single-threaded event loop that handles synchronous code, microtasks (Promises), and macrotasks (setTimeout, setInterval). Predict the exact output order and explain the reasoning.

---

## Code Snippet

```javascript
console.log("Start");
setTimeout(() => console.log("Timeout"), 0);
Promise.resolve().then(() => console.log("Promise"));
console.log("End");
```

---

## Requirements

1. **Predict the output order** (list the exact sequence).
2. **Explain why Promise beats setTimeout** (1-2 lines).
3. **Draw/describe the event loop flow** for this code.
4. **Identify the queue types:** Which queue handles setTimeout? Which handles Promise?

---

## Deliverable

Provide your answer in this format:

```
Output Order:
1. [first output]
2. [second output]
3. [third output]
4. [fourth output]

Why Promise beats setTimeout:
[explanation]

Event Loop Breakdown:
[describe the flow]

Queue Information:
- setTimeout goes to: [answer]
- Promise.then() goes to: [answer]
```

---

## Hints

- Synchronous code executes first (call stack).
- Microtask queue (Promises) is checked before macrotask queue (setTimeout).
- Even with `setTimeout(..., 0)`, it doesn't execute immediately.
