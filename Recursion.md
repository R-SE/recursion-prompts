Recursion is when a function or subroutine calls itself repeatedly.
- Termination condition: necessary in the case that data isn't validated and we get passed or reach a value that should throw an error
- Base case: condition in which function returns a value instead of recursing
  - can be thought of as the "base" or lowest level, otherwise we'd keep falling down the rabbit hole of recursion
- Recursive case: the clause where the function calls itself

```
let factorialize = n => {
  if (n < 0) return null            // terminating condition
  if (n < 2) return 1               // base case
  return n * factorialize(n - 1)    // recursive case
}
```

Opportunities to use recursion:
- look for cases where task is repeated multiple times because solving it will lead to multiple subtasks of the same kind
- in other words, we break a big task into smaller, equal tasks
