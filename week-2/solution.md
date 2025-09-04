# Solutions: The Problem Solver Developer's Challenge

---

## Stage 1: Digital Library Management:

A digital library.

```javascript
let bookTopic = prompt("Choose a book topic: ");
let bookScore = +prompt("What is the rating of the book?: ");

if (bookScore > 7) {
  alert(`You can have ${bookTopic} book.`);
} else if (bookScore < 7 && bookScore > 5) {
  let userRank = prompt("What is your rank?: ").toLowerCase();
  if (userRank === "vip") {
    alert(`You can have ${bookTopic} book.`);
  } else {
    alert(`You cannot have ${bookTopic} book.`);
  }
} else {
  alert(`You cannot have ${bookTopic} book.`);
}
```

---

## Stage 2: Online Food Order Management:

You are responsible for programming an online food ordering system.

```javascript
let food = prompt("Choose a food: pizza / burger / salad").toLowerCase();
let finalFood;

switch (food) {
  case "pizza":
    let pizzaType = prompt(
      "What type of pizza do you want? Pepperoni / Margarita / Vegetarian"
    ).toLowerCase();
    switch (pizzaType) {
      case "pepperoni":
        finalFood = "Pepperoni Pizza";
        break;
      case "margarita":
        finalFood = "Margarita Pizza";
        break;
      case "vegetarian":
        finalFood = "Vegetarian Pizza";
        break;
      default:
        finalFood = "Unknown Pizza";
    }
    alert(`You ordered: ${finalFood}`);
    break;
  case "burger":
    let burgerType = prompt(
      "What type of burger do you want? Cheeseburger / Veggie Burger / Chicken Burger"
    ).toLowerCase();
    switch (burgerType) {
      case "cheeseburger":
        finalFood = "Cheeseburger";
        break;
      case "veggie burger":
        finalFood = "Veggie Burger";
        break;
      case "chicken burger":
        finalFood = "Chicken Burger";
        break;
      default:
        finalFood = "Unknown Burger";
    }
    alert(`You ordered: ${finalFood}`);
    break;

  case "salad":
    let saladType = prompt(
      "What type of salad do you want? Caesar / Green Salad / Fruit Salad"
    ).toLowerCase();
    switch (saladType) {
      case "caesar":
        finalFood = "Caesar Salad";
        break;
      case "green salad":
        finalFood = "Green Salad";
        break;
      case "fruit salad":
        finalFood = "Fruit Salad";
        break;
      default:
        finalFood = "Unknown Salad";
    }
    alert(`You ordered: ${finalFood}`);
}
```

---

## Stage 3: Automated Grading System:

A teacher wants to design an automated grading system.

```javascript
let score = +prompt("What is the students score? out of 100");
let completion;

if (score > 90) {
  alert("Grade A");
} else if (score > 80 && score < 90) {
  alert("Grade B");
} else if (score >= 70 && score < 80) {
  completion = confirm("Is the project complete?");
  if (completion === true) {
    alert("Grade C+");
  } else {
    alert("Grade C");
  }
} else {
  alert("Failed");
}
```

---

## Stage 4: Banking System Simulation:

A bank has a system.

```javascript
let credit = 30000;
let action = prompt(
  "What action do you want to take? Balance / Withdrawal / Deposit"
).toLowerCase();
let amount;

switch (action) {
  case "balance":
    alert(`Your credit is ${credit}$`);
    break;
  case "withdrawal" || "withdraw":
    amount = +prompt("Please enter the amount of withdrawal: ");
    if (amount > credit) {
      alert(`Withdrawal amount (${amount}$) is bigger than credit ${credit}$`);
    } else {
      credit -= amount;
      alert(
        `Operation successful ${amount}$ was removed to your credit, new credit amount: ${credit}$`
      );
    }
    break;
  case "deposit":
    amount = +prompt("Please enter the amount of deposit: ");
    credit += amount;
    alert(
      `Operation successful ${amount}$ was added to your credit, new credit amount: ${credit}$`
    );
    break;
}
```

---

<div align="center">
  <b>Review these solutions and try to understand each step! 💡</b>
</div>
