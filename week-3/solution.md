# Solutions: The Problem Solver Developer's Challenge

---

## Stage 1: Even or Odd?:

Is the number Even or Odd?

```javascript
function oddOrEven(number) {
  return number % 2 === 0 ? "Even" : "Odd";
}
const number = +prompt("Enter a number: ", 7);
alert(oddOrEven(number));
```

---

## Stage 2: Which One is Larger?:

Which number is greater?

```javascript
const bigNumber = (arr) => {
  //   return Math.max(...arr);  Easy way
  let max = 0;
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] > max) {
      max = arr[i];
    }
  }
  return max;
};
console.log(bigNumber([3, 5, 7, 2, 8]));
```

---

## Stage 3: Dynamic Welcome Message:

Welcome Ashkan Sadeghi!

```javascript
function welcome(name, lastName) {
  return `Hello, ${name} ${lastName}. Welcome!`;
}

const name = prompt("Enter your name: ", "Ashkan");
const lastName = prompt("Enter your last name: ", "Sadeghi");
alert(welcome(name, lastName));
```

---

## Stage 4: Up to Ten!:

Multiply the number up to 10!

```javascript
function multiplicationTillTen(number) {
  for (let i = 1; i < 10; i++) {
    console.log(`${number} * ${i} = ${number * i}`);
  }
}
const multiplyNumber = +prompt("Enter a number to multiply: ", 3);
multiplicationTillTen(multiplyNumber);
```

---

## Stage 5: How Many Characters?:

How many characters does the word "Hello" have?

```javascript
function showCharacterCount(word) {
  const wordArr = word.split("");
  return wordArr.length();
}
const word = prompt("Enter word to count characters: ", "Hello");
alert(showCharacterCount(word));
```

---

## Stage 6: Is it Prime?:

Is the number Prime?

```javascript
function primeNumber(number) {
  if (number <= 1) return false;
  let prime = false;
  for (let i = 2; i < number; i++) {
    if (number % i === 0) {
      prime = false;
    } else {
      prime = true;
    }
  }
  return prime;
}
const prime = +prompt("Enter a number to check if it's prime: ", 7);
alert(primeNumber(prime) ? "It's a prime number" : "It's not a prime number");
```

---

## Stage 7: Whats the GCD?:

What is the GCD of these two numbers?

```javascript
function gcd(num1, num2) {
  while (num2 !== 0) {
    let temp = num2;
    num2 = num1 % num2;
    num1 = temp;
  }
  return num1;
}
const number1 = +prompt("Enter first number: ", 48);
const number2 = +prompt("Enter second number: ", 18);
alert(`GCD is ${gcd(number1, number2)}`);
```

---

## Stage 8: How Old Are You?:

Enter you birth year and I will tell you how old you are!

```javascript
function birthCalculator(number) {
  const currentYear = new Date().getFullYear();
  return currentYear - number;
}
const birthYear = +prompt("Enter your birth year: ", 1990);
alert(`You are ${birthCalculator(birthYear)} years old.`);
```

---

## Stage 9: Make It Reversed!:

What is the reversed version of "Hello"?

```javascript
function reverseString(str) {
  return str.split("").reverse().join("");
}
const stringToReverse = prompt("Enter a string to reverse: ", "Hello");
alert(reverseString(stringToReverse));
```

---

## Stage 7: Lets Count!:

Can a computer count to one million?

```javascript
function countOneToTen() {
  for (let i = 1; i <= 10; i++) {
    console.log(i);
  }
}
countOneToTen();
```

---

<div align="center">
  <b>Review these solutions and try to understand each step! 💡</b>
</div>
