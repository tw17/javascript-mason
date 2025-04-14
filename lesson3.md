# 🎓 JavaScript Basics – Tutorial 3: Making Decisions with If/Else

Now that you know variables and math, let's learn how your program can **make decisions** using **if/else statements**.

---

## 🤔 What are Conditional Statements?

In programming, we often need to run different code based on different situations.

An **if statement** lets your program decide whether to run some code.

Think of it like asking a question: "If something is true, then do this."

## Step 1: Create a New File
1. Open VS Code.
2. Inside your js-fun folder, create a new file called `decisions.js`.

## Step 2: Write a Simple Decision
Add this code to decisions.js:
```javascript
let playerScore = 50;

if (playerScore >= 50) {
  console.log("You passed the level!");
}
```
▶️ Run it
In the terminal, type: `node decisions.js`
You should see:
```
You passed the level!
```

## Step 3: Add an Else Option
Let's make a more complex decision with `else`:

```javascript
let playerScore = 45;

if (playerScore >= 50) {
  console.log("You passed the level!");
} else {
  console.log("Try again! You need 50 points to pass.");
}
```
▶️ Run it
You should see:
```
Try again! You need 50 points to pass.
```

## Step 4: Multiple Conditions
We can check multiple conditions with `else if`:

```javascript
let weather = "rainy";

if (weather === "sunny") {
  console.log("Wear sunscreen!");
} else if (weather === "rainy") {
  console.log("Bring an umbrella!");
} else if (weather === "snowy") {
  console.log("Wear a warm coat!");
} else {
  console.log("Check the weather forecast!");
}
```

## Try This Challenge
Create a file called `grade.js` with code that:
1. Creates a variable for a test score (0-100)
2. Uses if/else if/else to print the letter grade:
   - 90-100: "A"
   - 80-89: "B" 
   - 70-79: "C"
   - 60-69: "D"
   - Below 60: "F"

### Bonus
Change your program to ask "Did you do extra credit?" and add 5 points if the answer is yes!