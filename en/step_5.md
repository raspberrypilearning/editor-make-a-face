## Rectangles

Change the function `ellipse` to instead call the function `rect`.

```python line_numbers="true" line_number_start="10" line_highlights="15"

def draw():
    # Put code to run every frame here
    background(255, 255, 255)  
    # Add code to draw your face here
    fill(255, 255, 0) 
    rect(
        screen_size/2, 
        screen_size/2, 
        100, 
        50
    )  
  
```

## Now run your code

Run your code and check that you now see a rectangle instead of an ellipse.
