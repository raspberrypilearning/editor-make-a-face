<h2 class="c-project-heading--task">Triangles</h2>

--- task ---
➡️ Practice drawing a triangle

--- /task --- 

Add code to draw a `triangle`. Each pair of values is an x,y coordinate for one of the points of the triangle.

--- code ---
---
language: python
line_numbers: true
line_number_start: 10
line_highlights: 15-19
---

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
  
--- /code ---

**Test:** Experiment with changing the coordinates, then run your code to see a triangle displayed by joining the dots at those coordinates.