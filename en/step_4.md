## Outlines

The outline of a shape is called the **stroke**.

➡️ Change the stroke colour and thickness, or remove it.

Before the code where you draw the ellipse, you can choose to set a colour and thickness.


```python line_numbers="true" line_number_start="14" line_highlights="15-16"
    fill(255, 255, 0) 
    stroke(255, 255, 255)  
    stroke_weight(3)
    ellipse(
        screen_size/2, 
        screen_size/2, 
        100, 
        50
    )  
    
```

If you prefer, you can remove the stroke and have no outline.

```python line_numbers="true" line_number_start="14" line_highlights="15"
    fill(255, 255, 0) 
    no_stroke()
    ellipse(
        screen_size/2, 
        screen_size/2, 
        100, 
        50
    )  
  
```

## Now run your code

Run your code and check that the shape outline changes, or disappears if you removed the stroke.
