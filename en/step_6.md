## Triangles

Add code to draw a `triangle`. Each pair of values is an x,y coordinate for one of the points of the triangle.

```python line_numbers="true" line_number_start="10" line_highlights="15-19"

def draw():
    # Put code to run every frame here
    background(255, 255, 255)  
    # Add code to draw your face here
    fill(255, 255, 0) 
    triangle(
        210, 250, 
        330, 150, 
        220, 160
    )  
  
```

## Now run your code

Run your code and check that a triangle is drawn using the coordinates you chose.
