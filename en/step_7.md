## Positioning shapes

➡️ Position an ellipse or rectangle by changing the x,y coordinates of its centre point.

The first two values for `ellipse` and `rectangle` represent the x, y coordinates of its centre. Change the values to alter where it appears on the screen. 

```python line_numbers="true" line_number_start="11" line_highlights="17-18"

def draw():
    # Put code to run every frame here
    background(255, 255, 255)  
    # Add code to draw your face here
    fill(255, 255, 0) 
    rect(
        80, 
        60, 
        100, 
        50
    )  
  
```

> [!TIP]
>
> The top left corner of the screen is coordinate 0,0. Increasing the first number will move the shape to the right. Increasing the second number will move the shape downwards.

## Now run your code

Run your code and check that the shape moves when you change its coordinates.
