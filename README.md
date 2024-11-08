# Dynamic Mondrian Art Animation Project

## Overview

This project is an interactive digital artwork inspired by the style of Piet Mondrian, featuring dynamic shapes that move and animate over time. The artwork is created using the p5.js library.

## **Interactive Instructions**

​	When the page loads, the artwork will start moving automatically across the screen, triggering an animated effect. The artwork will experience edge bounces on the screen, and whenever the bounce is triggered, the display state of the cat's eyes and other related graphics will change, similar to the "death state".

​	When the painting touches the edge of the screen, the cat's eyes "flash" to give the effect of "death". The change in the eyes updates every time it hits the wall, adding to the visual interaction.

## **Personal Animation Method**

**Time-Based:**  Employ timers and events for animation.

## **Animation Properties**

​	The position of the painting and the display state of the cat's eye are the main attributes of animation. When the painting hits the edge of the screen, it bounces and changes direction, and the display state of "catevent1", "catevent2" and the cat's eye are switched, causing the cat to appear in a "dead" state.

​	The difference from the other team members is that this work pays more attention to position movement and shape display/hide state changes.

## **Sources of Inspiration**

​	My design was inspired by the classic game Snake. In Snake, the snake dies if it touches a wall. My work borrows on this mechanism, and whenever the painting touches the edge of the screen, the cat's eyes switch to the display state, showing a change similar to the state of death, and the effect of "death" is enhanced by switching the display state.

## Features

- **Dynamic Canvas**: The canvas adjusts to the window size, ensuring the artwork looks good on any device.
- **Interactive Shapes**: Shapes within the artwork move and bounce off the edges of the canvas, creating a lively and engaging visual experience.
- **Cat Animation**: These include a playful cat face that turns into a "dead" state when the canvas bounces.
- **Responsive Design**: The artwork scales and repositions itself when the window is resized, maintaining its aesthetic appeal.

## How It Works

### Initialization

- The `setup` function initializes the canvas, creates an instance of the `Artwork` class, and generates the initial artwork.
- The `createArtwork` function adds various shapes to the artwork, including rectangles, circles, lines, semicircles, triangles, and a dotted rectangle.

### Drawing and Updating

- The `draw` function continuously updates the canvas, displaying the current state of the artwork.
- The `windowResized` function ensures the artwork scales correctly when the window size changes.

### Shape Class

- The `Shape` class defines individual shapes with properties like position, size, color, and movement speed.
- Shapes can be of different types: rectangle, circle, line, semicircle, triangle, or dotted rectangle.

### Artwork Class

- The `Artwork` class manages a collection of shapes, providing methods to add, scale, and display them.
- The `scaleShapes` method adjusts the size and position of shapes when the window is resized.

### Animation

- The `startAnimation` function initiates a loop that updates the positions of all shapes every 20 milliseconds.
- Shapes bounce off the edges of the canvas, and specific shapes (like the cat's eyes) toggle their visibility to create a "winking" effect.

## Customization

- **Add New Shapes**: Modify the `createArtwork` function to add more shapes or change existing ones.
- **Adjust Movement**: Modify the `speedX` and `speedY` variables to change the speed of the shapes.
- **Change Colors**: Update the colors and styles of the shapes in the `Shape` class.

## Dependencies

- **p5.js**: A client-side JavaScript framework for creative coding.

## Acknowledgments

- Inspired by the works of Piet Mondrian.
- Utilizes the p5.js library for easy and efficient visual programming.

