<h2 class="c-project-heading--task">Face shape</h2>

➡️ Draw and colour a circle.

<h2 class="c-project-heading--explainer">Follow these instructions</h2>

An **ellipse** is an oval shape. If you specify the same width and height, you will draw a circle.  

Add code to the `draw()` function to set the fill colour in the same way as before using red, green and blue values.

Then, draw a circle in this colour.

<div class="c-project-code">

--- code ---
---
language: python
line_numbers: true
line_number_start: 10
line_highlights: 14-20
---

def draw():
    # Put code to run every frame here
    background(255, 255, 255)  
    # Add code to draw your face here
    fill(255, 255, 0) 
    ellipse(
        screen_size/2, 
        screen_size/2, 
        200, 
        200
    )  
  
--- /code ---

</div>

### Tip

<div class="c-project-callout c-project-callout--tip">

Make sure that the fill colour of your ellipse is not the same colour as your background.

</div>

## Now run your code

You should see a coloured circle.

Confirm the observable result.
