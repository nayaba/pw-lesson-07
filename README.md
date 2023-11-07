![that-way](https://github.com/nayaba/pw-lesson-07/assets/9198401/129a157e-e08d-4a05-a645-af1c2b7894ad)

# Introduction to Control Structures

Alright, ready to take control of your code? Let's chat about control structures in JavaScript. These are like the GPS of your code—they help you decide which way to go, depending on the conditions at hand.

### 1. If, Else-If, Else: Choosing Your Adventure

Imagine you're in one of those choose-your-own-adventure books. You hit a fork in the story:

- If you choose to go left, turn to page 42.
- If you choose to go right, turn to page 18.
- Else (if you just can't decide), you stay put and read a footnote.

That's your basic `if`, `else if`, `else` structure:

```javascript
let road = 'left';

if (road === 'left') {
  console.log("You've arrived at a mysterious cave.");
} else if (road === 'right') {
  console.log("You've stumbled upon a hidden beach.");
} else {
  console.log("You're still at the crossroads, undecided.");
}

// If you run this code snippet you should see the below output in your console:
// "You've arrived at a mysterious cave."
```

### 2. Switch: The Control Tower

The `switch` statement is like having a control tower that directs airplanes (different cases) to the correct runway based on their flight number (the expression):

```javascript
let weather = 'sunny';

switch (weather) {
  case 'rainy':
    console.log("Don't forget an umbrella!");
    break;
  case 'sunny':
    console.log("Grab your sunglasses!");
    break;
  case 'snowy':
    console.log("Time for a snowball fight!");
    break;
  default:
    console.log("Hmm, let's just stay inside.");
}

// If you run this code snippet you should see the below output in your console:
// "Grab your sunglasses!"
```

`break;` is like telling the plane, "Okay, you've landed, you can stop now." The `default` case is like saying, "If the weather is something weird, just default to staying indoors."

### 3. For Loop: The Conveyor Belt

A `for` loop is like a conveyor belt that repeats a process a set number of times. You tell it where to start the count, where to end, and how to step through items:

```javascript
for (let i = 0; i < 5; i++) {
  console.log("Package number " + i + " is on the belt.");
}

// If you run this code snippet you should see the below output in your console:
// Package number 0 is on the belt.
// Package number 1 is on the belt.
// Package number 2 is on the belt.
// Package number 3 is on the belt.
// Package number 4 is on the belt.
```

### 4. While Loop: Circling the Block

A `while` loop keeps circling the block until some condition is no longer true. It'll keep going as long as the condition is `true`:

```javascript
let fuel = 5;

while (fuel > 0) {
  console.log("The car is still running. Fuel level: " + fuel);
  fuel--;
}

// If you run this code snippet you should see the below output in your console:
// The car is still running. Fuel level: 5
// The car is still running. Fuel level: 4
// The car is still running. Fuel level: 3
// The car is still running. Fuel level: 2
// The car is still running. Fuel level: 1
```

### 5. Do-While Loop: At Least Once

The `do-while` loop is like saying, "I'm going to drive through the neighborhood at least once, even if I realize partway through that I don't need to be here":

```javascript
let doIWantIceCream = false;

do {
  console.log("I'm getting ice cream regardless!");
} while (doIWantIceCream);

// If you run this code snippet you should see the below output in your console:
// "I'm getting ice cream regardless!"
```

The code block will run once before the condition is checked.

### 6. Break and Continue: Hitting the Brakes or Skipping a Step

- `break` jumps out of the loop entirely.
- `continue` skips the rest of the current iteration and jumps to the next one.

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 3) {
    continue; // Skip number 3!
  }
  if (i === 7) {
    break; // Stop the loop entirely when we hit 7
  }
  console.log(i);
}

// If you run this code snippet you should see the below output in your console:
// 0
// 1
// 2
// 4
// 5
// 6
```

### Practice Time!

Let's put you in the driver's seat. Head over to CodePen and create a simple program that loops through numbers 1 to 10 and prints whether each number is even or odd. Here's a hint: `%` (the modulus operator) might be helpful here.

```javascript
for (let i = 1; i <= 10; i++) {
  if (i % 2 === 0) {
    console.log(i + " is even");
  } else {
    console.log(i + " is odd");
  }
}
```

Go ahead, type it out, and watch the magic happen in your console!

### Recap and What's Next

You've just had a whirlwind tour of control structures in JavaScript! Like any good tour, there's always more to see and do. But for now, soak up the sights and sounds of `if` statements, `switch` cases, and loops. Play around with them, mix them up, and see what happens. And remember, in coding, the best way to learn is by doing. So, go out there and write some awesome code! 🚀

[Back to the Wiki](https://github.com/nayaba/pw-wiki)
