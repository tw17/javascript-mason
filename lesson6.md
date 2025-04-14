# 🎓 JavaScript Basics – Tutorial 6: Objects - Grouping Data Together

Now that you understand variables, decisions, loops, and functions, let's learn about **objects** – a powerful way to group related information together!

---

## 📦 What are Objects?

Objects are containers that hold related data and functions. They help us organize our code like putting related things into a labeled box.

In real life, a car object would have:
- Properties: color, brand, model, year
- Methods (functions): start(), stop(), turn()

## Step 1: Create a New File
1. Open VS Code.
2. Inside your js-fun folder, create a new file called `objects.js`.

## Step 2: Your First Object
Add this code to objects.js:

```javascript
// Create a player object
let player = {
  name: "SpaceExplorer",
  health: 100,
  level: 1,
  isAlive: true
};

// Access object properties using dot notation
console.log("Player name: " + player.name);
console.log("Health: " + player.health);
console.log("Level: " + player.level);
```

▶️ Run it
In the terminal, type: `node objects.js`

## Step 3: Changing Object Properties
Objects are flexible - you can change their values:

```javascript
let player = {
  name: "SpaceExplorer",
  health: 100,
  level: 1
};

console.log("Player starts at level " + player.level);

// Player levels up!
player.level = 2;
player.health = 120;

console.log("Player is now level " + player.level);
console.log("Player now has " + player.health + " health");

// You can even add new properties
player.weapon = "Laser Sword";
console.log("Player found a " + player.weapon);
```

## Step 4: Objects with Methods
Objects can also have their own functions (called methods):

```javascript
let dog = {
  name: "Buddy",
  breed: "Golden Retriever",
  age: 3,
  
  // This is a method - a function inside an object
  bark: function() {
    console.log("Woof woof!");
  },
  
  // Another method that uses the object's own properties
  introduce: function() {
    console.log("Hi! I'm " + this.name + ", a " + this.age + "-year-old " + this.breed);
  }
};

// Call the methods
dog.bark();
dog.introduce();
```

## Step 5: Objects in Arrays and as Function Parameters
Objects are very flexible - you can put them in arrays and pass them to functions:

```javascript
// Array of game character objects
let characters = [
  { name: "Wizard", power: "Magic", health: 50 },
  { name: "Warrior", power: "Strength", health: 100 },
  { name: "Archer", power: "Precision", health: 75 }
];

// Function that works with character objects
function printCharacter(character) {
  console.log("Character: " + character.name);
  console.log("Power: " + character.power);
  console.log("Health: " + character.health);
  console.log("------------------------");
}

// Loop through each character and print their details
for (let i = 0; i < characters.length; i++) {
  printCharacter(characters[i]);
}
```

## Try This Challenge
Create a file called `videogame.js` that:
1. Creates a game character object with properties like name, health, items, etc.
2. Adds methods to the character that make it:
   - Take damage (reduces health)
   - Use a healing potion (increases health)
   - Add an item to inventory
3. Use these methods in a simple game scenario

### Bonus Challenge
Create multiple character objects and put them in an array to make a simple team. Then create a function that finds and returns the character with the highest health on the team.