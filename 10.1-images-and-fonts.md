# 10.1-images-and-fonts

## Step 1: Load the Image

To use an image, you need to preload it using the `preload()` function. This function is called before the `setup()` function and ensures the image is fully loaded before the program starts.

1. Place your image file in the same directory as your sketch.
2. make a variable to hold your image 
3. Use the `loadImage()` function inside `preload()` to load the image.
 
  -`createImg()` 

```javaScript
let img;

function preload() {
  img = loadImage('imageName.jpg'); // Replace with your image file path
}
```

## Step 2: Display the Image

In the `setup()` or `draw()` function, use the `image()` function to display the image on the canvas.

```javaScript
function setup() {
  createCanvas(800, 600); // Create a canvas
}

function draw() {
  background(220); // Set a background color
  image(img, 0, 0); // Display the image at coordinates (0, 0)
}
```

## Step 3: Adjust Image Properties

You can adjust the position, size, and other properties of the image using additional parameters in the `image()` function.

```javaScript
function draw() {
  background(220);
  image(img, 50, 50, 200, 200); // x,y,w,h
}
```

## Step 4: Working with Multiple Images

To work with multiple images, repeat the preload and display steps for each image.

```javaScript
let img1, img2;

function preload() {
  img1 = loadImage('path/to/your/image1.jpg');
  img2 = loadImage('path/to/your/image2.jpg');
}

function setup() {
  createCanvas(800, 600);
}

function draw() {
  background(220);
  image(img1, 0, 0, 200, 200);
  image(img2, 220, 0, 200, 200);
}
```

## Tips
- Use image formats supported by web browsers (e.g., JPG, PNG, GIF).
- Experiment with image functions like `tint()`, `filter()`, and `resize()` to manipulate your images further.

# Fonts
