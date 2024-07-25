> Note: THIS FILE WILL BE UPDATED FREQUENTLY!! 

## Alternative to _consol.log_ 
> NOTE: this part was copied from another person, I don't remember their name to credit them. But thank you anyway!

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
> PERSONAL NOTES

## Operations

- The `**` operator.
  - mass / (height \* height) IS THE SAME AS => mass / (height \*\* 2).

## String Interpolation

```js
let fName = "conan";
let lName = "7x";

let fullName = `My name is ${fName} ${lName}`;
```

## String

Backticks can be used to write normal strings.

In JS to write a string we can use `""` OR `''` OR ` ``(backtick) `

Using backticks:

- we don't need to use `/n`, we can write multiple lines with putting any sign for creating a new line.

## Type Conversion

- `Number()`
- `String()`
- `Boolean()` 

### Type Coercion
The type the JS converts automatically (behind the scenes)

## Truthy and Falsy Values
5 falsy values: 
- `0`
- `''` (Empty String)
- `undefined` 
- `null`
- `NaN`

## Methods
`prompt()` works similarly to `alert()` but it allows the user to enter a value, which returns it as a _**string**_ 
> Don't judge my variable naming ( I'm just practicing here XD )

![image](https://github.com/ZYMNZ/JS_Notes/assets/98342638/c63992cb-c888-4ddd-b4ca-5acbeb59a137)

## Equality Operators: == vs. ===
`==` and `!=` is the _loose_ version of equality

`===` and `!==` is the _strick_ version of equality

## Strict mode
It should be written at the top.

![image](https://github.com/user-attachments/assets/0dcbcf51-bc7b-4fee-b44e-c0df1e7b4a16)

## Types of Functions 

### Function Declaration
- The function can be called before writing it.
  
![image](https://github.com/user-attachments/assets/3eef7c14-df69-4b92-8bd8-67e72445ebfb)

### Function Expression
![image](https://github.com/user-attachments/assets/24124ee9-02ad-4f39-bfce-1b9e6e86c411)

### Arrow function 
> Can't be called in a `this` keyword (To be confirmed)
#### one param (optional) with a single line of code
![image](https://github.com/user-attachments/assets/8c15e9f3-420f-49a2-b22d-461fbb54fb66)
![image](https://github.com/user-attachments/assets/9fb97e56-51d9-4ca6-b688-422b6e1a3535)

#### one param but more than one line of code, we use `{}`
![image](https://github.com/user-attachments/assets/e5334470-a238-4dcc-8dd8-507f1cbf5af6)

#### more than one param
- we use parenthesis `()` to wrap the params 

![image](https://github.com/user-attachments/assets/f6457965-9136-4c38-be03-0cc49407bf9d)

REVISION:

![image_2024-07-24_194310791](https://github.com/user-attachments/assets/d2d69ba5-addf-402e-8f8d-cb2dd95335c1)

## Arrays 
```js
const friends = ['Conan', 'Candl3'];
```
- `friends.push('Twin');` will add it to the end of the array (return the array length)
- `friends.unshift('Twin');` will add it to the start of the array (return the array length)
- `friends.pop();` will remove the last element of the array (return the removed element)
- 
