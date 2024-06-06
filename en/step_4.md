<h2 class="c-project-heading--task">Outlines</h2>

--- task ---
The outline of a shape is called the **stroke**.

➡️ Change the stroke colour and thickness, or remove it.

--- /task --- 

Before the code where you draw the ellipse, you can choose to set a colour and thickness.


--- code ---
---
language: python
line_numbers: true
line_number_start: 14
line_highlights: 15-16
---
    fill(255, 255, 0) 
    stroke(255, 255, 255)  
    stroke_weight(3)
    ellipse(
        screen_size/2, 
        screen_size/2, 
        100, 
        50
    )  
    
--- /code ---

If you prefer, you can remove the stroke and have no outline.

--- code ---
---
language: python
line_numbers: true
line_number_start: 14
line_highlights: 15
---
    fill(255, 255, 0) 
    no_stroke()
    ellipse(
        screen_size/2, 
        screen_size/2, 
        100, 
        50
    )  
  
--- /code ---

**Test:** Experiment with changing the stroke colour and thickness or removing it, then run your code to see the results. 