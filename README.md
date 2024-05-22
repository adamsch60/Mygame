# Space Shooter Game

## Introduction

This game runs on Windows. It has been tested at a resolution of 1980x1060p, but it should adapt to different screen sizes.

## Gameplay

The player controls a spaceship and must stop incoming enemy ships by shooting them with the left mouse button. The objective is to destroy the enemy ships.

### Starting the Game

- The game begins at the start screen.
- Press any key to start the game.

### Player Interface

The player's health and score are displayed in the top left corner of the screen. Press the <kbd>P</kbd> key to pause the game. In the pause screen, only the player's ship is visible to prevent exploiting the pause function. Press any key to resume the game.

## Enemies

### Types of Enemies

At the start, there are 5 types of enemy ships:




1. **Type 1:**
   - Medium speed.
   - Fires in front at medium intervals.
   <p align="center">
       <img src="./Spacegame/textures/enemy1.png" height="200"/>
   </p>
2. **Type 2:**
   - Slow speed.
   - Fires towards the player at long intervals.
    <p align="center">
    <img src="./Spacegame/textures/enemy2.png" height="200"/>
    </p>
3. 3. **Type 3:**
   - Fast speed.
   - Does not shoot.
   <p align="center">
       <img src="./Spacegame/textures/enemy3.png" height="200"/>
   </p>
4. **Type 4:**
   - Slow speed, moves laterally.
   - Creates a drone similar to Type 1 at long intervals.
   <p align="center">
       <img src="./Spacegame/textures/enemy4.png" height="200"/>
    </p>
5. **Type 5:**
   - Slow speed, moves laterally.
   - Fires a laser beam at long intervals that damages the player upon contact.
   <p align="center">
       <img src="./Spacegame/textures/enemy5.png" height="200"/>
   </p>
### Enemy Behavior

- These 5 enemy types appear in random order and increase in speed over time.
- Destroying an enemy ship grants 10 points.
- Destroying a drone grants 3 points.

### Player Damage

The player can take damage in the following ways:

- Allowing an enemy ship to reach the bottom of the screen: **-3 life points**
- Colliding with an enemy ship: **-5 life points**
- Getting hit by an enemy projectile: **-1 life point**
- Passing through a laser beam: **-2 life points**
- Colliding with a drone: **-3 life points**
- Allowing a drone to pass: **-1 life point**

## Boss Battles

<p align="center">
    <img src="./Spacegame/textures/boss.png" height="300"/>
</p>

- Upon reaching 500 points, a boss enemy appears.
- The boss is destroyed after 50 hits, with each successful hit awarding 10 points.
- The boss uses 3 random attacks:
  1. Fires a screen-wide laser array at the player at short intervals.
  2. Fires a large laser beam while tracking the player's movement.
  3. Fires 2 small homing missiles that disappear after a short time or can be destroyed by the player.

### Post-Boss Gameplay

- After defeating the boss, faster small enemies will appear until the player reaches another 500 points, at which point a new boss will appear.

## Game Over

- When the player dies, the final score is displayed.
- The game will close 3 seconds after displaying the score.

## Things to Improve

These are features I would add if I had unlimited time, not in order of importance:

- Implementing a custom coordinate system (not based on the screen).
- Local high score table.
- Boss life counter.
- Visual representation of damage.
- Adjustable frame rate (FPS).
- Moving configuration settings to a separate file.
- More boss attacks.
- More types of spaceships (e.g., bombers that leave bombs behind, laser net ships functioning as nodes of a laser grid).
- Upgrades for the player’s ship (e.g., more cannons, extra life, screen clear).
- More starting ships (e.g., ships with more life but slower cannons, laser-beam-shooting ships with less life).
- Improved hitboxes.
- Better formula for increasing enemy spawn frequency.
- Background visuals.
- Storyline.
- Extensive playtesting.
