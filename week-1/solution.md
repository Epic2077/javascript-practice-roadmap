# Solutions: The Novice Developer's Challenge

---

## Stage 1: Introduce Yourself to the Teacher

Ask the user for their first name, last name, and age, then display in the console.

```javascript
let firstName = prompt("Enter your first name:");
let lastName = prompt("Enter your last name:");
let age = prompt("Enter your age:");

console.log("First Name:", firstName);
console.log("Last Name:", lastName);
console.log("Age:", age);
```

---

## Stage 2: Understanding Differences

Display the differences between `let`, `var`, and `const` in the console.

```javascript
console.log("Differences between var, let, and const:");
console.log(
  "var: Function-scoped or globally-scoped. Can be redeclared and updated."
);
console.log(
  "let: Block-scoped. Cannot be redeclared in the same scope, but can be updated."
);
console.log(
  "const: Block-scoped. Cannot be redeclared or updated. Must be initialized during declaration."
);
```

---

## Stage 3: Mirror Look

Get two inputs and display them in reverse order.

```javascript
let input1 = prompt("Enter the first value:");
let input2 = prompt("Enter the second value:");

console.log("Mirrored Inputs:", input2, input1);
// To reverse the strings themselves:
// console.log("Mirrored Inputs:", input1.split('').reverse().join(''), input2.split('').reverse().join(''));
```

---

## Stage 4: Mathematical Calculations

Get a number and display negation, 20th power, Boolean value, and remainder when divided by 2.

```javascript
let num = parseFloat(prompt("Enter a number:"));

console.log("Negation (-num):", -num);
console.log("20th Power (num^20):", num ** 20);
console.log("Boolean Value (Boolean(num)):", Boolean(num));
console.log("Remainder when divided by 2 (num % 2):", num % 2);
```

---

## Stage 5: Naming Variables

Assign suitable names and data types.

```javascript
let userName = "John Doe"; // string
const piValue = 3.14159; // number
const googleDomain = "https://www.google.com"; // string
let userId = 12345; // number (or string if alphanumeric)
let delayDurationInMs = 2000; // number (milliseconds)
```

---

## Stage 6: Determining Data Types

Identify the data types of the following values:

| Value                           | Data Type | Description                              |
| ------------------------------- | --------- | ---------------------------------------- |
| "Pizza"                         | string    | Text value                               |
| 3 + 2                           | number    | 5                                        |
| "4" + 4                         | string    | "44" (concatenation)                     |
| 122222332232322232323232232321n | bigint    | Large integer                            |
| 5 \|\| 1                        | number    | 5 (logical OR returns first truthy)      |
| 5 && 0                          | number    | 0 (logical AND returns first falsy)      |
| 5 \* "33"                       | number    | 165 (string coerced to number)           |
| null                            | object    | typeof null is "object" (historical bug) |

---

## Stage 7: Age Confirmation

Ask for age, confirm, and display a message.

```javascript
let userAge = prompt("Enter your age:");
let isAgeCorrect = confirm(`You entered ${userAge}. Is this correct?`);

isAgeCorrect && alert("You are " + userAge + " years old");
```

---

## Stage 8: Code Execution Order

**Explanation:**
Scripts are loaded and executed by the browser in the order they appear in the HTML document (`<script>` tags). This is synchronous by default. The browser pauses HTML parsing to fetch (if external) and execute each script in sequence before moving on to the next one. Using the `async` or `defer` attributes changes this behavior for external scripts.

---

## Stage 9: Expression Output

Predict the output of the following expressions:

```javascript
let item = 3; // item is 3
const temp = ++item; // item becomes 4, temp is 4
item = temp++; // item is 4, then temp becomes 5

let stars = " *** "; // stars is " *** "
stars = 2 + " *** " * 3; // " *** " * 3 is NaN, so 2 + NaN is NaN

let flag = false; // flag is false
flag = flag++; // flag remains false
```

---

## Stage 10: Math Question

Ask a math question and check the answer.

```javascript
let question = "12 + 2 = ?";
let answer = prompt(question);
Number(answer) === 14 && alert("Won!");
Number(answer) !== 14 && alert("Game Over!");
```

---

## Stage 11: Even or Odd Number

Check if a number is even or odd and display the result.

```javascript
let number = parseInt(prompt("Enter a number:"));

num % 2 === 0 && alert("Even Number")(num % 2 !== 0) && alert("Odd Number");
```

---

<div align="center">
  <b>Review these solutions and try to understand each step! 💡</b>
</div>
