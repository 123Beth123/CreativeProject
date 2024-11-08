# 动态蒙德里安艺术动画项目

## **Individual Task**

**Time-Based:**  Employ timers and events for animation.



## Overview

This project is an interactive digital artwork inspired by the style of Piet Mondrian, featuring dynamic shapes that move and animate over time. The artwork is created using the p5.js library, which provides a JavaScript environment for visual arts.

## Features

- **Dynamic Canvas**: The canvas adjusts to the window size, ensuring the artwork looks good on any device.
- **Interactive Shapes**: Shapes within the artwork move and bounce off the edges of the canvas, creating a lively and engaging visual experience.
- **Cat Animation**: A playful cat's face is included, with eyes that can "dead" when the canvas bounces.
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

## Usage

1. **Clone the Repository**:

   ```
   git clone https://github.com/yourusername/mondrian-artwork.git
   cd CreativeProject
   ```

2. **View the Artwork**:

   - Open your web browser and navigate to `http://localhost:5500` (or the port specified by the server). 注意，请确保在VSCode中打开Live Server。

## Customization

- **Add New Shapes**: Modify the `createArtwork` function to add more shapes or change existing ones.
- **Adjust Movement**: Modify the `speedX` and `speedY` variables to change the speed of the shapes.
- **Change Colors**: Update the colors and styles of the shapes in the `Shape` class.

## Dependencies

- **p5.js**: A client-side JavaScript framework for creative coding.

## Acknowledgments

- Inspired by the works of Piet Mondrian.
- Utilizes the p5.js library for easy and efficient visual programming.

