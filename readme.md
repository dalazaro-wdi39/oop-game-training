Creator: Daryl Lazaro
Location: SF

![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)

# Training: Model a Game with OOP

You've learned about OOP, but let's look at how to **incorporate object oriented programming patterns into a web site**.  This document has an example of how we might approach making a card-matching memory game.

### Deliverable

Design user stories, data structures, development stories, and potential challenges for a **racing game** in which two players use the keyboard to control "cars" that race across the screen.

Here are some popular bonus features that would affect your data structure plan:

1. How would you make your player's "cars" use custom images?
2. Can a player type in their name to see custom win messages?
3. Can you enable a reset button to restart the race?
4. How about a win counter that spans across multiple races?

As you work, you can edit this README to add a section at the top with your name, a link to the original repository, and a 3-5 sentence reflection on completing this assignment. Push your updates to GitHub and add a link to the repo to the "My Work" section of your website!

### User Stories & Game Mechanics
1. A user will be able to use their keyboard to steer a uniquely colored car.
2. Users (2+ players) will see their car scrolling across the screen, bottom to top.
3. Users will be notified via marker if their car is traveling in the wrong direction (top to bottom, i.e. reverse).
4. The first user to cross a finish line is deemed the 1st place winner!
5. Other users will be ranked the order in which they cross the finish line (2nd, etc).

### Data Structures for "Memory" (Independent Practice)
Let's consider object types Car, Racetrack, and Game.

* List the type of each property (number, boolean, `Card`, etc.).
* List the parameters that each method will take.
* Don't forget a constructor!

**Car**
  - `carPlayer` (number)
  - `carColor` (string)
  - `isleader` (boolean)
  - `isMovingForward()` (Function - declare on-screen that player is traveling in reverse)
  - `topSpeed` (number)
  - `currentSpeed` (number)
  - `accelerate(currentSpeed, topSpeed)` (Function)
  - `brake(currentSpeed, topSpeed)` (Function)
  - `Car(options)` (Function)

**Racetrack**
  - `startingLine` (number)
  - `finishLine` (number)
  - `Map()` (Function - constructor, create a map object with different properties)

**Game**
  - `steering(key1, key2, key 3, etc)` (Function - listening for keyDown/keyUp events on keyboard)
  - `leaderboard` (array of numbers)
  - `reset()` (Function - resets the game!)
  - `reverse()` (Function - detect if player is traveling in reverse)
  - `Game(number of Cars)` (Function - constructor)
  - `hasCrossed()` (Function - check if a user has crossed the finish line)
  - `podium()` (Function - check who placed 1st, 2nd, etc)
  - `results()` (Function - display a win message)

###Potential Challenges / Development Questions

1.


