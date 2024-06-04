<h2 class="c-project-heading--task">Change the size</h2>

--- task ---
Change the size of the ellipse.

--- /task --- 
 
Change the size of the ellipse by changing the width and height values to different numbers. 

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

<div class="c-project-callout c-project-callout--tip">

### Tip

If you set the width or height to a number larger than the `screen_size`, your ellipse will not fit on the screen.

</div>

**Test:** Run your code and you should see the ellipse change size.











--- /task ---

--- task ---

**Test:** Run your code and change it to get the face size and shape that you want.

--- /task ---

--- task ---

Choose a stroke colour for the outline and a fill colour for the main part of the shape.

[[[processing-stroke]]]

If you don't want an outline, then use `no_stroke()`.

--- code ---
---
language: python
filename: main.py - draw()
line_numbers: true
line_number_start: 13
line_highlights: 14
---

    # Add code to draw your face here
    fill(255, 255, 0)  # Bright yellow
    ellipse(width/2, height/2, 200, 200)
  
--- /code ---

[[[generic-theory-simple-colours]]]

--- /task ---

--- task ---

**Test:** Run your code and change the colour until you are happy with it.

--- /task ---

--- save ---
