# Task 2: Hundreds of Bubbles

In this task, you will create the animation of bubbles rising in a bottle.
Here is an example of the output we are expecting (this one has a sketch size of 200 x 500).

<img src="../images/bubbles.gif">

## Specifications

Here are some guidelines for how you should do this:

- We are expecting you to commit your work often (try to aim for a minimum of 3-5 commits per lab) with useful commit messages marking your progress.

- Create a bubble class with:
    - Attributes: `x,y,radius,speedY`
    - Constructor: 
        - `x` = random value from 0 to the sketch width
        - `y` = random value from height+50 to height+750
        - `radius` = random value from 1 to 10
        - `speedY` = -10/radius
    - `move()` function:  
        - x-location randomly changes within -0.8 and 0.8
        - y-location is incremented speedY 
        - Once a bubble goes above the top edge of the sketch, its attributes are assigned new set of random values (similar to how they were set in the constructor).
    - `display()` function
        - Draw an ellipse representing the bubble.
        - Create an array with 250 bubbles, then move and display them in the animation loop.

- Challenge (this is optional):
    - Update your code so that we only have a maximum of 12 big bubbles at any time (size of bubbles: small is from 1 to 3, big is 10 to 15)

## Embed an animated gif of your drawing
 
Embed the animated gif you created here using markdown syntax: `![alt text of image](relative path to image)`