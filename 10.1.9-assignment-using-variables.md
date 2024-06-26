# 10.1.9-assignment-using-variables

## Working with Basic Variables
 
Be sure to run each part before moving on to the next. As you go, add comments that give a title to each activity.


## Set Up
- Make your display window 800, 1000 with a background color of your choice.
- Fonts are not required but you are welcome to use them.


# Part 1: Volume - Calculating Volume with Variables (40%)
- Add a comment to your code to give this section of code a title. I recommend using a format such as:  `//*********************** Part 1 - Volume *******************`
- Your task will be to calculate the volume of air in this classroom in cubic feet.
The room is about 29 feet wide, 37 feet long and 12 feet high. To do this, follow  the steps below.
---- 


1.  ## Set up the dimensions of the room
  - Create three variables called w, l, and h to store the width, length, and height.
     - (Note: the words `width` and `height` are reserved words in P5 that store the size of the canvas so you need to use `w` and `h` instead.)
- Tech Moment: We will be working with whole numbers for this part. Remember that whole numbers are stored as a data type known as Integer.
Store the numbers in the variables as described in the paragraph above.  



2. ## Prepare to Calculate the Volume
  - Create a variable called volume.
  - Use a math formula to store the volume in the variable.
     - As a reminder, volume = length * width * height.
     - You must have the computer do the math using the three variables from step 1.
As a reminder, we did some simple math in an in-class example


3. ## Print the Result
  - Use a text line to print out your final statement such as:
     - Room W101 contains a lot of hot air.  (approximately ___ cubic feet of air).

---

# Part 2: Time Table - Using String Variables (50%)

- Before moving on to part 2, fix your indenting to line everything up properly.
- Add a comment to your code to give this section of code a title. I recommend using a format such as:  `//*********************** Part 2 - Timetable *******************`
- Your task will be to create your class timetable using variables to store the teacher names and their courses. To do this, follow  the steps below.


1. ## Set up the Variables
- Store the names of all of your teachers in four separate variables called teacher1, teacher2, teacher, and teacher4.
  - Remember that words, in this case the teacher names, must be indicated in “double quotes”.
Store the names of all the courses in variables called `course1`, `course2`, `course3`, and `course4`.  
- Tech Moment: Words are stored as a data type known as String.

Did you do this right?  You should now have **8 separate** variables, each with words already stored in them.

2. ## Draw the timetable
- Using lines and/or rectangles, you will set up a grid for a 1 semester timetable.  This will essentially be a 2x5 table (or something similar)
- Create a rectangle with a black stroke and an orange fill.  The size and location are up to you but be sure to it big enough to fit in your timetable
- Change your stroke to black and then draw lines to create the grid within your rectangle. 
colours are optional

3. ## Use text() statements that use the above variables to print out the information into the timetable. One possible layout is the following: 
|  | Class |
| ----------- | ----------- |
| Block 1 | Calm |
| Block 2 | Math 10 |
| Block 3 |  |
| Block 4 | |
| Block 5 |  |

Did you do this right?  The words “Block 1” are not stored in a variable so you should print them out directly in the text line.  The teachers and the courses are stored in variables so you should have used those variables in your text lines.


# Part 3 - Final 10 %

- Before moving on to part 3, fix your indenting to line everything up properly.
- Add a comment to your code to give this section of code a title. I recommend using a format such as:  `//*********************** Part 3 - Final 10% MOD *******************`


## Have you ever heard of the math operator called `MOD`?  
`MOD` uses the % sign and it means divide but it gives the REMAINDER.
- For example:
  -  8 % 2 = 0
  -  8 % 3 = 2
  -  8 % 5 = 3

Learn about modulo [here](https://www.freecodecamp.org/news/javascript-modulo-operator-how-to-use-the-modulus-in-js/)

Here is the challenge.  If I ran a race for 252 seconds, how many minutes and how many seconds did it take me. 
1. ## Use the divide and the MOD operator and print out the results in some way below your table.



