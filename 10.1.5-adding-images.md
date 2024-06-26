# 10.1.5-adding-images
Graded

## How to short version
1. save image
   - stick to .png or .gif or .jpg
   - rename them to have short names
   - do not have any spaces in the name
3. upload into P5
4. There are 3 steps to load images:

   - set up variables to hold images `let img1`
   - make `function preload()` load the images into the variables  
   - draw to screen using `image()`


# Displaying SpongeBob and Friends on an Ocean Background
1. Find Images:

     - Find images of SpongeBob, Patty, Patrick, and one more character that you'd like to display in your p5.js sketch. Make sure you have these image files saved and ready for use.
     - you can use any of your favorite childhood tv shows.
  
3. Declare Variables:

   - Declare variables to hold the loaded images for SpongeBob, Patty, Patrick, and the additional character. Also, create a variable to control SpongeBob's jitter effect:
`let spongeBob;`

5. Load Images in `preload()`:

   - Load the images in the `preload()` function. Remember to copy the correct file path for your images.
```javaScript
function preload() {
  spongeBob = createImg("spongebob.jpg","anything can go here");
}//end preLoad
```

4. Draw Images on the Screen:

   - In the `draw()` function, draw the loaded images on the canvas. You can use the `image()` function for each character:
```javaScript
function draw() {
  image(spongeBob, x,y,w,h);
}
```

## todo:
1. Ocean Background

   - The background color has been set to represent an ocean background with a blue color. You can adjust the background colors to your preference. OR find an image to use as the background 

2. Jitter Effect:

   - SpongeBob's position is given a jitter effect using the `random()` function to add random values to his x and y coordinates. The goal is to make him look like he has had just a little too much coffee. You can adjust the jitter variable to control the intensity of the jitter effect.
3. A little theory

   - in a comment at the top of your code, tell me the difference between JPEG, GIF, and PNG. Also, tell me how many colors each file type supports. 
