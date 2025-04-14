# 🎓 JavaScript Basics – Tutorial 4: Loops - Doing Things Over and Over

Now that you can make decisions in your code, let's learn about **loops** – a way to repeat code without typing it multiple times.

---

## 🔄 What are Loops?

Loops let you run the same code multiple times. This is useful when you need to do something repeatedly, like:
- Counting from 1 to 10
- Doing something for each player in a game
- Repeating an action until something happens

## Step 1: Create a New File
1. Open VS Code.
2. Inside your js-fun folder, create a new file called `loops.js`.

## Step 2: Your First Loop - The For Loop
Add this code to loops.js:

```javascript
// This counts from 1 to 5
for (let count = 1; count <= 5; count++) {
  console.log("Count is: " + count);
}
```

▶️ Run it
In the terminal, type: `node loops.js`
You should see:
```
Count is: 1
Count is: 2
Count is: 3
Count is: 4
Count is: 5
```

### How the For Loop Works:
```javascript
for (let count = 1; count <= 5; count++) {
// ↑               ↑           ↑
// Start count at 1 Keep going  Add 1 each time
//                 while count  (count++ means
//                 is <= 5      count = count + 1)
```

## Step 3: The While Loop
Another way to create loops is using `while`. This keeps running as long as a condition is true:

```javascript
let rockets = 3;

while (rockets > 0) {
  console.log(rockets + "... ");
  rockets = rockets - 1;
}

console.log("Blast off! 🚀");
```

▶️ Run it
You should see:
```
3... 
2... 
1... 
Blast off! 🚀
```

## Step 4: Loop Through an Array
Arrays are lists of items. We can loop through them:

```javascript
let fruits = ["apple", "banana", "orange", "grape"];

console.log("My fruit basket has:");

for (let i = 0; i < fruits.length; i++) {
  console.log("- " + fruits[i]);
}
```

▶️ Run it
You should see:
```
My fruit basket has:
- apple
- banana
- orange
- grape
```

## Try This Challenge
Create a file called `stars.js` that:
1. Uses a loop to draw a triangle pattern of stars like this:
```
*
**
***
****
*****
```
Hint: You'll need a loop inside a loop!

### Bonus Challenge
Create a countdown timer that counts from 10 to 1, waits one second between each number, and then says "Happy New Year!" at the end.
Hint: Look up `setTimeout` in JavaScript!