# README


## Udacity Instructions

Students should use this [rubric](https://review.udacity.com/#!/projects/2696458597/rubric) for self-checking their submission. Make sure the functions you write are **object-oriented** - either class functions (like Player and Enemy) or class prototype functions such as Enemy.prototype.checkCollisions, and that the keyword 'this' is used appropriately within your class and class prototype functions to refer to the object the function is called upon. Also be sure that the **readme.md** file is updated with your instructions on both how to 1. Run and 2. Play your arcade game.

For detailed instructions on how to get started, check out this [guide](https://docs.google.com/document/d/1v01aScPjSWCCWQLIpFqvg3-vXLH2e8_SZQKC8jNO0Dc/pub?embedded=true).

## Pre-start Notes
- to build the game, I need to edit `app.js`
- no need to edit `js/resources.js` or `js/engine.js`
- the list below still leaves a lot out.  Really dig in and see what's missing and how I would actually
implement it

### This is what I need to do:
- The Enemy function, which initiates the Enemy by:
  - Loading the image by setting this.sprite to the appropriate image in the image folder (already provided)
    - CM => already done
  - Setting the Enemy initial location (you need to implement)
  - Setting the Enemy speed (you need to implement)
- The update method for the Enemy
  - Updates the Enemy location (you need to implement)
  - Handles collision with the Player (you need to implement)
- You can add your own Enemy methods as needed

- The Player function, which initiates the Player by:
  - Loading the image by setting this.sprite to the appropriate image in the image folder (use the code from the Enemy function as an example on how to do that)
  - Setting the Player initial location
- The update method for the Player (can be similar to the one for the Enemy)
- The render method for the Player (use the code from the render method for the Enemy)
- The handleInput method, which should receive user input, allowedKeys (the key which was pressed) and move the player according to that input. In particular:
  - Left key should move the player to the left, right key to the right, up should move the player up and down should move the player down.
  - Recall that the player cannot move off screen (so you will need to check for that and handle appropriately).
  - If the player reaches the water the game should be reset by moving the player back to the initial location (you can write a separate reset Player method to handle that).
- You can add your own Player methods as needed.

Once you have completed implementing the Player and Enemy, you should instantiate them by:

- Creating a new Player object
- Creating several new Enemies objects and placing them in an array called allEnemies

