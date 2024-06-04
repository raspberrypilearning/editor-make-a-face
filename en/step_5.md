<h2 class="c-project-heading--task">Rectangles</h2>

--- task ---
You can draw other shapes. Practice drawing a rectangle.

--- /task --- 

Change the function `ellipse` to instead call the function `rect`.

--- code ---
---
language: python
line_numbers: true
line_number_start: 10
line_highlights: 15
---

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
  
--- /code ---

**Test:** Change the function name, then run your code to see a rectangle instead of an ellipse.