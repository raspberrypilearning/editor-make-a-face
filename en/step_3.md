## Change the size

➡️ Make the circle larger or smaller, or create an oval shape by making one of the dimensions larger than the other.

Change the width and height values to see the ellipse change shape. 

```python line_numbers="true" line_number_start="10" line_highlights="18-19"

def draw():
    # Put code to run every frame here
    background(255, 255, 255)  
    # Add code to draw your face here
    fill(255, 255, 0) 
    ellipse(
        screen_size/2, 
        screen_size/2, 
        100, 
        50
    )  
  
```

> [!TIP]
>
> If you set the width or height to a number larger than the `screen_size`, your ellipse will not fit on the screen.

## Now run your code

Run your code and check that the ellipse changes size.
