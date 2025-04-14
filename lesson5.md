# 🎓 JavaScript Basics – Tutorial 5: Functions - Create Your Own Commands

Now that you know about variables, decisions, and loops, let's learn about **functions** – a way to create your own custom commands in JavaScript!

---

## 🧩 What are Functions?

Functions are blocks of code that:
- Have a specific job
- Can be used over and over
- Run only when you call them
- Can take inputs and return outputs

Think of functions like creating your own special powers in your program!

## Step 1: Create a New File
1. Open VS Code.
2. Inside your js-fun folder, create a new file called `functions.js`.

## Step 2: Your First Function
Add this code to functions.js:

```javascript
// Define a function
function sayHello() {
  console.log("Hello, welcome to my program!");
}

// Call (use) the function three times
sayHello();
sayHello();
sayHello();
```

▶️ Run it
In the terminal, type: `node functions.js`
You should see the greeting printed three times!

## Step 3: Functions with Parameters
Let's make our function more useful by giving it inputs (called parameters):

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}

greet("Mason");
greet("Dad");
greet("Buddy");
```

▶️ Run it
You should see personalized greetings for each name!

## Step 4: Functions with Return Values
Functions can also give back (return) a value:

```javascript
function addNumbers(a, b) {
  return a + b;
}

let sum = addNumbers(5, 3);
console.log("The sum is: " + sum);

// You can also use the returned value directly
console.log("10 + 20 = " + addNumbers(10, 20));
```

## Step 5: Combining Functions with Other Concepts
Let's use functions with if statements and loops:

```javascript
function checkGameScore(score) {
  if (score >= 100) {
    return "You win a gold medal!";
  } else if (score >= 50) {
    return "You win a silver medal!";
  } else {
    return "Keep practicing!";
  }
}

// Let's test our function with different scores
let scores = [30, 70, 120];

for (let i = 0; i < scores.length; i++) {
  let currentScore = scores[i];
  let result = checkGameScore(currentScore);
  console.log("Score: " + currentScore + " - " + result);
}
```

## Try This Challenge
Create a file called `calculator.js` that:
1. Has four functions: `add()`, `subtract()`, `multiply()`, and `divide()`
2. Each function should take two parameters and return the result
3. Test each function with some example values
4. Bonus: Add error checking to the `divide()` function that prevents division by zero

### Super Bonus Challenge
Create a simple "Rock, Paper, Scissors" game using functions:
1. Make a function that randomly chooses rock, paper, or scissors for the computer
2. Make a function that determines the winner between player and computer choices
3. Make a function that runs a game and displays the results