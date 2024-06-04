<h2 class="c-project-heading--task">Face shape</h2>

--- task ---
Draw and colour a shape for your face or mask. 

![Image of a square-faced robot.](images/robot-teeth.png){:width="200px"}
--- /task --- 
 
![Examples of different faces.](images/strip.png)

Add code to the `draw()` function to draw the outline of a face.

<div class="c-project-code">


--- code ---
---
language: python
line_numbers: true
line_number_start: 10
line_highlights: 14
---

def draw():
    # Put code to run every frame here
    background(255, 255, 255)  
    # Add code to draw your face here
    ellipse(screen_size/2, screen_size/2, 200, 200)  
  
--- /code ---

</div>

**Test:** Run your code and you should see a coloured square. 

![The output area showing a black line circle in the middle of the grid.](images/black-circle.png)

