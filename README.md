## Alternative to consol.log
`console.dir()`

For hierarchical listing of arrays and objects.
```js
console.dir(["apples", "oranges", "bananas"]);
```
![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/fcf2bb44-5c3b-4e44-8f50-1d5fb53bb76b)

`console.table()`

For rows and columns listing of arrays (might not be suitable for objects).
```js
console.table(["apples", "oranges", "bananas"]);
```
![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/511d3736-24de-488d-a022-4d5c1635d68f)
```js
console.table({"a": 1, "b": 2, "c": 3});
```

![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/1a005ed2-ba31-4a15-b32e-5ce3cc3810d2)


# JS NOTES UDEMY CLASS

## Operations

- The `**` operator.
  - mass / (height \* height) IS THE SAME AS => mass / (height \*\* 2).

## String Interpolation

```js
let fName = "conan";
let lName = "7x";

let fullName = `My name is ${fName} ${lName}`;
```

### String

Backticks can be used to write normal strings.

In JS to write a string we can use `""` OR `''` OR ` ``(backtick) `

Using backticks:

- we don't need to use `/n`, we can write multiple lines with putting any sign for creating a new line.

### Type Conversion


