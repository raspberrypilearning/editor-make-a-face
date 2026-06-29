<h2 class="c-project-heading--task">Change the size</h2>

➡️ Make the circle larger or smaller, or create an oval shape by making one of the dimensions larger than the other.

<h2 class="c-project-heading--explainer">Follow these instructions</h2>

Change the width and height values to see the ellipse change shape. 

<div class="c-project-code">

--- code ---
---
language: python
line_numbers: true
line_number_start: 10
line_highlights: 18-19
---

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
  
--- /code ---

</div>

### Tip

<div class="c-project-callout c-project-callout--tip">

If you set the width or height to a number larger than the `screen_size`, your ellipse will not fit on the screen.

</div>

## Now run your code

You should see the ellipse change size.

Run your code and check that the ellipse changes size.
