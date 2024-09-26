## INTERMEDIATE CONCEPTS IN JAVASCRIPT

## Nullish Coalescing Operator (??)

- `Definition`: The ?? operator returns the right-hand operand when the left-hand operand is null or undefined. Otherwise, it returns the left-hand operand.

- `Where to Apply`: When you want to provide a default value for variables that might be null or undefined without overriding other falsy values (like 0, '', or false).

- `How to Apply`: Use the operator to check if a variable is null or undefined and assign a fallback/default value.

`Syntax:`

```java script
let result = value1 ?? value2;
```

`Example Code:`

```java script
let userName = null;
let displayName = userName ?? "Guest";
console.log(displayName); // Output: "Guest"

let count = 0;
let displayCount = count ?? 10;
console.log(displayCount); // Output: 0

```

## Optional Chaining (?.)

``Definition`:` The ?. operator allows you to safely access deeply nested properties of an object without having to manually check each level for null or undefined.

`Where to Apply:` When accessing nested properties, elements in arrays, or methods that might not exist, to prevent runtime errors.

`How to Apply:` Use the ?. operator at each property or method level where null or undefined might occur.

`Syntax:`

```javascript
object?.property;
object?.[expression];
object?.method?.();
```

`Example Code :`

```javascript
let user = { profile: { name: "Alice" } };

let userName = user?.profile?.name;
console.log(userName); // Output: "Alice"

let userCity = user?.address?.city;
console.log(userCity); // Output: undefined
```

## type of

`Definition:`
The typeof operator evaluates a value and returns a string indicating the type of the unevaluated operand.

`Syntax:`

```javasript
typeof operand

```

`operand`: The value or expression whose type you want to check. This can be a variable, object, or any valid JavaScript expression.

## Common Return Values of typeof:

- "undefined": If the value is `undefined`.
- "boolean": If the value is a boolean `(true or false)`.
- "string": If the value is a `string`.
- "number": If the value is a `number`.
- "bigint": If the value is a `BigInt`.
- "symbol": If the value is a s`ymbol`.
- "function": If the value is a `function`.
- "object": If the value is an `object`, including arrays and null.

### When and Where to Use:

**Type Checking**: You can use typeof to check if a variable has been initialized or to verify the type of input data.

**Error Handling:** It is useful for debugging or preventing errors by checking if a variable is of the expected type before performing operations on it.

**Conditional Statements:** It can be used in conditions to apply different logic depending on the data type.

```javascript
console.log(typeof undefined); // "undefined"
console.log(typeof 42); // "number"
console.log(typeof "hello"); // "string"
console.log(typeof true); // "boolean"
console.log(typeof { a: 1 }); // "object"
console.log(typeof [1, 2, 3]); // "object" (arrays are also objects)
console.log(typeof null); // "object"
console.log(typeof function () {}); // "function"
console.log(typeof Symbol()); // "symbol"
console.log(typeof BigInt(123)); // "bigint"
```
