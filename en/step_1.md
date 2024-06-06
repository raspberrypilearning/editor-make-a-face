<h2 class="c-project-heading--task">Choose a background colour</h2>

--- task ---
➡️ Think of an idea for the kind of face or mask you want to make.

➡️ Set up your image by choosing a background colour.
--- /task --- 
 
![Examples of different faces.](images/strip.png)

The three numbers in `background(0, 0, 0)` are red, green and blue values. Experiment with changing the numbers to any whole number between 0 and 255 to change the background colour. 

<div class="c-project-code">
--- code ---
---
language: python
line_numbers: true
line_number_start: 10
line_highlights: 12
---
 
def draw():   
    # Put code to run every frame here
    background(0, 0, 0)    
  
--- /code ---
</div>

**Test:** Run your code and you should see a coloured square. 

<div class="c-project-callout c-project-callout--tip">

### Tip

For a white background, choose `background(255, 255, 255)`.

</div>
