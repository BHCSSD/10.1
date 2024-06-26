# 10.1.8-rotation-and-translation
S&T

---
## Rotations in p5.js

Rotations in p5.js are achieved using the `rotate()` function, which rotates the shape around the origin (0, 0) or around a point you specify. The rotation angle is measured in radians by default. You can use the `radians()` function to convert degrees to radians if needed.

### Step-by-Step Guide

1. **Setting Up the Environment**  
   First, set up the basic p5.js environment with `setup()` and `draw()` functions.

   ```javascript
   function setup() {
     createCanvas(400, 400);
     angleMode(RADIANS); // Use radians for rotation angles
   }

   function draw() {
     background(220);
   }
   ```

2. **Translating the Origin**  
   To rotate an object around its center, you need to translate the origin to the center of the object before rotating it. This is done using the `translate()` function.

   ```javascript
   function draw() {
     background(220);

     // Translate to the center of the canvas
     translate(width / 2, height / 2);
   }
   ```

3. **Rotating the Shape**  
   Use the `rotate()` function to rotate the shape. The angle of rotation is specified in radians.

   ```javascript
   function draw() {
     background(220);

     // Translate to the center of the canvas
     translate(width / 2, height / 2);

     // Rotate by 45 degrees (PI / 4 radians)
     rotate(PI / 4);

     // Draw a rectangle at the origin (which is now the center of the canvas)
     rectMode(CENTER);
     rect(0, 0, 100, 50);
   }
   ```

4. **Animating the Rotation**  
   To create an animation, you can increment the rotation angle in the `draw()` loop.

   ```javascript
   let angle = 0;

   function draw() {
     background(220);

     // Translate to the center of the canvas
     translate(width / 2, height / 2);

     // Rotate by the current angle
     rotate(angle);

     // Draw a rectangle at the origin (which is now the center of the canvas)
     rectMode(CENTER);
     rect(0, 0, 100, 50);

     // Increment the angle for animation
     angle += 0.01;
   }
   ```

5. **Combining with Other Transformations**  
   You can combine rotation with other transformations like `scale()` and `translate()` to create more complex animations.

   ```javascript
   let angle = 0;

   function draw() {
     background(220);

     // Translate to the center of the canvas
     translate(width / 2, height / 2);

     // Rotate by the current angle
     rotate(angle);

     // Scale the shape
     scale(1.5);

     // Draw a rectangle at the origin (which is now the center of the canvas)
     rectMode(CENTER);
     rect(0, 0, 100, 50);

     // Increment the angle for animation
     angle += 0.01;
   }
   ```

6. **Resetting Transformations**  
   Use `push()` and `pop()` functions to save and restore the transformation states. This is useful when you want to apply transformations to specific shapes without affecting others.

   ```javascript
   let angle = 0;

   function draw() {
     background(220);

     // First shape
     push();
     translate(width / 2, height / 2);
     rotate(angle);
     rectMode(CENTER);
     rect(0, 0, 100, 50);
     pop();

     // Second shape without transformations
     rect(50, 50, 100, 50);

     // Increment the angle for animation
     angle += 0.01;
   }
   ```

### Summary
- **`translate(x, y)`**: Moves the origin to a new location.
- **`rotate(angle)`**: Rotates shapes around the current origin.
- **`angleMode()`**: Sets the mode for measuring angles (`RADIANS` or `DEGREES`).
- **`push()` and `pop()`**: Save and restore the transformation states to isolate transformations.

By combining these functions, you can create complex and animated rotations in p5.js.

---


```
function setup() {
  createCanvas(800, 800);
  angleMode(DEGREES);
  rectMode(CENTER);
}
function draw() {
  background(220);
    rectMode(CENTER);
    //move the origin point

    rotate(45);             
    //draw at new origin point

    resetMatrix();          //sets origin and rotate back to normal

    rectMode(CORNER);
    rect(400, 400, 100, 100);

}
function mousePressed() { 
print("MouseX: " + mouseX + "     MouseY: " + mouseY);
} //end mousePressed

```
