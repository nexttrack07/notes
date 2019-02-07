## Implicit Coercion: Strings & Numbers

The `+` operator is overloaded. It can be either addition or concatenation. When it either one of it's arguments is a string, it concatenates.
The `-` is not overloaded. It coerces either or both of its arguments to numbers.
The `==` prefers to compare numbers. This means that it will coerce either or both values to a number and then compare them.

```javascript
if ("123" == true) return true // this does not return true because it compares the number 123 to the number 1
```

### When to use double equals?

- Can either value be _true_ or _false_?
- Can either value every be `[]` or `""` or `0`?

\*\* In The above cases, do not use `==`. Prefer `===` instead.
