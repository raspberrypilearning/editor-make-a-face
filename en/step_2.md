<h2 class="c-project-heading--task">Face shape</h2>

--- task ---
Draw and colour a shape for your face or mask. 

--- /task --- 
 
Add code to the `draw()` function to set the fill colour in the same way as before using red, green and blue values.

Then, draw an ellipse (oval) in this colour.

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

<div class="c-project-callout c-project-callout--tip">

### Tip

Make sure that the fill colour of your ellipse is not the same colour as your background.

</div>

**Test:** Run your code and you should see a coloured circle.


