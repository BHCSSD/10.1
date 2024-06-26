### 10.1.3-adding-text
 Graded
 # How to write them words

 Our goal with this example is to make text and have it zoom past
  
  
  ## TODO:
  ## Part 1: 60%
  1. Make a new File with `10.1.3-adding-text` as the name 
  2. Check your `createCanvas(x, y)` inside of `setup()`. Set x to 600, and y to 400
  3. inside the `draw` function set your background colour to an r,g,b: `background();`  your choice
  4. add a box to the middle of the screen
  5. inside the box add `text("WORDS GO HERE",x,y)`
  6. Change the font size `textSize(12)` and make it BIG
  7. add `noStroke()` in the line before your text, use a comment `//` to tell me what it does
  9. add `fill(r,g,b)` change the colour of the text only
      
## Part 2: some problem solving 70%
  10. inside of your `text()` change your number for the x value to the variable `textX` (this was set on line 1 of the code, it is a variable)
  11. with the idea that `textX` is a variable and can be changed, how can you make the text scoot off the screen? hint: start with a new line `textX = textX` and use this to change the x value using grade 1 math.
  12. I was going to put the answer to #8 here, but I decided to be a bit mean... good luck

## Part 3: more advanced problem solving 90%
  13. to reset the `text()` back to the other side of your screen, you need an if statement. Copy and paste time:
```javaScript   
  if (   textX < -250     ){ // you will need to edit the. If your x is __________ 
    textX=500;// reset the `textX` to a new position
    print("too far to the right");
    }
````


## TODO2: 100% 
1. make 2 new variables at the top of the screen 
2. make a new line of text at the bottom left corner of the screen
3. using your 2 variables make the text go up in a diagonal line to the other corner 


## starter code
```javaScript
let textX = 250;

function setup() {
  createCanvas();
  
}

function draw() {
  background(255);

}
//reminder on how to draw different things
//  text("WORD",x,y)
//  fill(r,g,b);
//  stroke(r,g,b);
//  noStroke()
//  strokeWeight(13)
// writing secret messages
//  This can be used to "Comment out" a line so the computer will not read your message as code
```
