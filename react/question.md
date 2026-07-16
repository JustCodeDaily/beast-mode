# Day 1: React Component Prop Flow

## Difficulty
Beginner

## Topic
Unidirectional Data Flow & Props in React

## Objective
Understand why props are immutable and how to properly handle state changes.

---

## Task Description

In React, props flow from parent to child unidirectionally. Attempting to mutate a prop directly violates this principle and won't cause re-renders. Identify the issue and provide the correct solution.

---

## Code Snippet

```jsx
function Parent() {
  const [count, setCount] = React.useState(0);
  return <Child count={count} />;
}

function Child({ count }) {
  count = count + 1; // What happens?
  return <div>{count}</div>;
}
```

---

## Requirements

1. **Identify the problem:** What's wrong with modifying `count` directly in Child?
2. **Explain the consequence:** Why doesn't this trigger a re-render?
3. **Provide the correct solution:** How should Child handle the count change?
4. **Show the corrected code:** Write the working version.

---

## Deliverable

Provide your answer in this format:

```
Problem: [what's wrong]

Consequence: [why it fails]

Solution: [how to fix it]

Corrected Code:
[paste your working code here]
```

---

## Hints

- Props are read-only from the child's perspective.
- Mutations don't trigger React's re-render cycle.
- If the child needs to modify state, pass a callback from the parent.
