Link to discussion : 
[click here!](https://github.com/HamidrezaRahimian/Python-Programming/discussions)

__________________________________________________________________________________________________________


this is how you can get started with Turtle :
__________________________________________________________________________________________
Starting a turtle environment
In a Python shell, import all the objects of the turtle module:

`from turtle import` 
__________________________________________________________________________________________

__________________________________________________________________________________________
Basic drawing
Send the turtle forward 100 steps:

`forward(100)`
__________________________________________________________________________________________

`left(120)`
Let’s continue by drawing a triangle:

```
forward(100)
left(120)
forward(100)
```
Experiment with those commands, and also with backward() and right().
__________________________________________________________________________________________

Try changing the color - for example, color('blue') 
- and width of the line - for example, width(3) 
__________________________________________________________________________________________

The turtle’s position
Send your turtle back to its starting-point (useful if it has disappeared off-screen):

`home()`
The home position is at the center of the turtle’s screen. If you ever need to know them, get the turtle’s x-y co-ordinates with:

`pos()`
Home is at (0, 0)
__________________________________________________________________________________________
And after a while, it will probably help to clear the window so we can start anew:

`clearscreen()`
Making algorithmic patterns
__________________________________________________________________________________________
Using loops, it’s possible to build up geometric patterns:

```
for steps in range(100):
    for c in ('blue', 'red', 'green'):
        color(c)
        forward(steps)
        right(30)
```
- which of course, are limited only by the imagination!
__________________________________________________________________________________________
Let’s draw the star shape at the top of this page. We want red lines, filled in with yellow:

```
color('red')
fillcolor('yellow')
```
Just as up() and down() determine whether lines will be drawn, filling can be turned on and off:

`begin_fill()`
Next we’ll create a loop:

```
while True:
    forward(200)
    left(170)
    if abs(pos()) < 1:
        break
```
abs(pos()) < 1 is a good way to know when the turtle is back at its home position.

Finally, complete the filling:

`end_fill()`
(Note that filling only actually takes place when you give the end_fill() command.)

__________________________________________________________________________________________




<img width="330" alt="image" src="https://github.com/HamidrezaRahimian/Week-3-Phyton/assets/143603503/d2d10378-aa3a-4dcb-bdf1-95ce5137810b">







here is an example of full code :
-----------------------------------------------------------------------------------------------------------
#turtle graph lernen King Alex


```
import turtle

# Function to draw a square with the given side length
def draw_square(side_length):
    for _ in range(100):
        turtle.forward(side_length)
        turtle.right(90)

# Main function
def main():
    # Set up Turtle graphics
    turtle.speed(1)  # Set drawing speed
    turtle.color("blue")  # Set pen color

    # Set the side length of the square
    side_length = 100  # You can adjust the side length here

    # Call the draw_square function
    draw_square(side_length)

    # Keep the window open until clicked
    turtle.exitonclick()

# Check if the script is being run as the main program
if __name__ == "__main__":
    # Call the main function
    main()
```

