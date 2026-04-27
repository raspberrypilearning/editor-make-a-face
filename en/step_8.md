<h2 class="c-project-heading--task">Overlap shapes</h2>

➡️ Make shapes you couldn't otherwise create by overlapping shapes.

<h2 class="c-project-heading--explainer">Follow these instructions</h2>

You could add two overlapping circles to create a smile. Start with an ellipse to represent the face. 

--- code ---
---
language: python
line_numbers: true
line_number_start: 11
line_highlights: 15-16
---
def draw():
    # Put code to run every frame here
    background(125, 0, 125)
    # Add code to draw your face here
    fill(125, 75, 0) # Brown
    ellipse(200, 220, 150, 150) # Face
--- /code ---

Set the `fill` colour for your mouth then draw an `ellipse`. Set the `fill` colour again, this time to match the face colour, then draw a second `ellipse`.

Change the `y` coordinate of the second `ellipse` to a slightly higher position for a smile.

--- code ---
---
language: python
line_numbers: true
line_number_start: 11
line_highlights: 17-20
---
def draw():
    # Put code to run every frame here
    background(125, 0, 125)
    # Add code to draw your face here
    fill(125, 75, 0) # Brown
    ellipse(200, 220, 150, 150) # Face
    fill(255, 0, 0)  # Red
    ellipse(200, 240, 40, 40) # Mouth
    fill(125, 75, 0) # Brown
    ellipse(200, 235, 40, 40) # Overlap   

--- /code ---

## Now run your code

Experiment with changing the fill colours and sizes of the ellipses. Run your program to see the results.

Run your code and check that the overlapping ellipses make a smiling mouth.
