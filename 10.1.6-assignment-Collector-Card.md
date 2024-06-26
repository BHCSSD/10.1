# 10.1.6-assignment-Collector-Card
Assignment


# P5.js Assignment 2 - Collector Card

## Your job is to create one of the following:
- Sports card -or- a playing card using actors, your favorite band/singer, etc.
- Game card (pokemon, magic the Gathering, dnd)
- ID Card 
- A $21 bill for Hobbslandia

## Set Up
Create a new P5.js file and name the file 10.1.6-assignment-Collector-Card

If doing a traditional collector card, set your canvas size to 400,600.  For other cards or topics, you can choose your dimensions. 


# Marks 
## Base Requirements 50% - Your card must include the following:
- A variable to store the name of your person/character.
  - Every time you display that name on the screen, you **must** use the variable, rather than hard-coding in the text.  In other words, your text line should look like `text(nameVariable, 50, 50)` rather than `text(“Nugent-Hopkins”, 50,50)`
- a background colour
- a rectangle to indicate the shape of the card
  - Use the ROUNDED corner rectangle for a more professional look.  [Click here](https://p5js.org/reference/#/p5/rect) to learn about rounded rectangles
- THREE pictures
  - a picture of the person/character
  - Other pictures such as a  team logo, super-power indicator, etc.
- Two fonts plus at least 2 different sizes. Text ideas could include:
  - person’s name
  - facts or statistics
  - your company logo
  - [Click here](https://www.geeksforgeeks.org/p5-js-loadfont-function/) to see how to load fonts. It is very much like using images

## Layout and Design 20%
| Mark | Description |
| ----------- | ----------- |
| 5/20 | Shows very little attention to alignments, sizes, etc. |
| 10/20 | Demonstrates some attention to alignments, sizing, etc. |
| 15/20 | Makes a solid effort to make the product look good. |
| 20/20 | Layout is almost perfect.  Things are centered where appropriate, spacing is consistent, etc. |

## Final 30% - To get top marks, you must include:
- at least 4 different pictures
- TWO fonts are used with at least 4 changes in size.
- Additional Shapes or lines to further enhance the look of your card

# Extra Challenge (not for marks)
Add a `mousePressed()` function that shows the BACK of the card while you are holding the mouse button.

# Hints: 
- Do you know about `textAlign()`?
- Do not forget about `imageMode()`!
- Do not forget about `tint()` if you want to overlap some images
- `noStroke()` and  `noFill()` can also be useful
