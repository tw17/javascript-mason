# 🎓 JavaScript Basics – Tutorial 2: Variables and Math

Now that you’ve written your first program, it’s time to learn how to **store information** and do **math** in JavaScript using **variables**.

---

## 🧠 What is a Variable?

A **variable** is like a box that holds a value.

You give the box a name, and then you can use it later.

Example:

```javascript
let score = 10;
console.log(score);
```

This will print: `10`

## Step 1: Create a New File
1.	Open VS Code.
2.	Inside your js-fun folder, create a new file called math.js.

##  Step 2: Create and Use Variables
Add this code to math.js:
```javascript
let playerName = "Mason";
let score = 5;

console.log("Player: " + playerName);
console.log("Score: " + score);
```
▶️ Run it
In the terminal, type: `node math.js`
You should see:
```
Player: Mason
Score: 5
```

## Step 3: Math with Numbers
JavaScript can do math just like a calculator.

Replace your code with this:
```javascript
let apples = 5;
let bananas = 3;

let totalFruits = apples + bananas;

console.log("Total fruits: " + totalFruits);
```
You should see:
`Total fruites: 8`

### More Math Examples
```javascript
let a = 10;
let b = 2;

console.log("Add: " + (a + b));
console.log("Subtract: " + (a - b));
console.log("Multiply: " + (a * b));
console.log("Divide: " + (a / b));
```
Run it and look at the results in the terminal.
