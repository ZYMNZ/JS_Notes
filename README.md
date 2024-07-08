> Note: THIS FILE WILL BE UPDATED FREQUENTLY!! 

## Alternative to _consol.log_
### console.dir()

For hierarchical listing of arrays and objects.
```js
console.dir(["apples", "oranges", "bananas"]);
```
![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/fcf2bb44-5c3b-4e44-8f50-1d5fb53bb76b)

### console.table()

For rows and columns listing of arrays (might not be suitable for objects).
```js
console.table(["apples", "oranges", "bananas"]);
```
![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/511d3736-24de-488d-a022-4d5c1635d68f)
```js
console.table({"a": 1, "b": 2, "c": 3});
```

![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/1a005ed2-ba31-4a15-b32e-5ce3cc3810d2)

### console.group()
To create a new inline group in the console output, making it easier to organize and read related messages.
```js
console.log('This is the top outer level');

console.group('Task 1');
console.log('Task activity 1');
console.log('Task activity 2');
console.groupEnd();

console.group('Task 2');
console.log('Task activity 3');
console.log('Task activity 4');
console.groupEnd();

console.log('Back to the top outer level');
```

![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/d07f48a0-8d7a-4acd-9683-951a402ea7e5)

### console.time() & console.timeEnd()
To measure the duration of an asynchronous task
```js
try {
  console.time("record-1");
  await someAsyncTask();
} catch (error) {
   // handle error
} finally {
  console.timeEnd("record-1");
}
```
![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/70e7a3e2-3616-42be-8c71-fc6b315744ce)

### console.clear()

This will clear the console.


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

- `Number()`
- `String()`

### Type Coercion

The type the JS converts automatically (behind the scenes)

### Truthy and Falsy Values











