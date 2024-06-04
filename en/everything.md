

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







## Add eyes

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Eyes make a shape start to look like a face.
</div>
<div>
![The output area showing a face with eyes.](images/eyes.png){:width="200px"}
</div>
</div>

--- task ---

Think about what kind of eyes your face needs. The simplest eyes are just two circles. 

You could add different coloured irises and pupils. You could add light highlights / catchlights in a different colour. 

--- /task ---

Experiment with `ellipses` in the `draw` function to create the eyes you want. 

--- task ---

### Position the eyes

The first number in `ellipse` is the center of the eye. The eyes should be positioned the same distance from the centre of the drawing. 

In this example, `160` and `240` are both `40` pixels away from 200, which works for a drawing with a width of 400. 

--- code ---
---
language: python
filename: main.py - draw()
---
    fill(0, 0, 0)  # Black — change to red, green, or blue up to 255
    eye_size = 50
    ellipse(160, 180, eye_size, eye_size)  # x, y, width, height
    ellipse(240, 180, eye_size, eye_size)

--- /code --- 

**Tip:** If you want round eyes, then using an `eye_size` variable makes it easier to change the width and height of both eyes in one place.

[[[processing-python-ellipse]]]

--- collapse ---

---
title: Calculating positions based on width
---

The centre of a drawing is at position `width / 2` or half the width. You can use this to position the eyes by subtracting the eye width for the left eye and adding it for the right eye:

--- code ---
---
language: python
filename: main.py - draw()
---

    fill(0, 0, 0)  # Black — change to red, green, or blue up to 255
    eye_size = 50
    ellipse( (width / 2) - 40, 180, eye_size, eye_size)  # x, y, width, height
    ellipse( (width / 2) + 40 , 180, eye_size, eye_size)

--- /code ---

You could also calculate the width of the eyes based on the width of the drawing.

--- code ---
---
language: python
filename: main.py - draw()
---

    fill(0, 0, 0)  # Black — change to red, green, or blue up to 255
    ellipse( (width / 2) - (width / 10) , 180, eye_size, eye_size)  # x, y, width, height
    ellipse( (width / 2) + (width / 10) , 180, eye_size, eye_size)

--- /code ---

--- /collapse ---

Change the second number in the `ellipse` function call to move the `y` (vertical) position of the eyes. 

--- /task ---

--- task ---

**Test:** Keep changing the shape and position of the eyes until you like the way they look.

**Tip:** If you set a stroke for drawing the face and don't want one for the eyes, then you will need to call `no_stroke()` before drawing the eyes. 

[[[processing-stroke]]]

--- /task ---

--- task ---

### Add detail

You can use more circles to create:
+ Coloured irises
+ Black pupils
+ White catchlights
+ Or, something else

This eye has a coloured iris, black pupil, and white catchlights with changed opacity:
![The output area showing an eye with catchlights over the pupil and iris.](images/catchlights.png)

[[[generic-theory-simple-colours]]]
[[[processing-opacity]]]

You can also animate the eyes by rotating them.

[[[processing-rotation]]]

--- /task ---

--- task ---

**Test:** Keep changing the eyes until you like the way they look.

Is your drawing starting to look like a face? 

--- /task ---

--- task ---

**Debug:** You might find some bugs in your project that you need to fix. Here are some common bugs.

--- collapse ---
---
title: The eyes aren't centred
---

You could use `height / 2` to place them in the centre.

--- /collapse ---

--- collapse ---
---
title: The eyes aren't aligned with each other
---

If you want the eyes to be aligned, then make sure you use the same number for the coordinates for both eyes. Try using a variable so that the values are always the same. 

--- /collapse ---

--- collapse ---

---
title: I can't see the pupil or iris
---

The eye needs to be drawn first, then the iris, and finally the pupil. The order in which you draw things is very important.

Computer graphics are made of layers. In your eye, each ellipse is a layer. Objects on higher layers sit in front of objects on lower layers. Imagine cutting all the shapes out of paper. Depending on how you arrange and overlap that paper, the final result could look very different.

--- /collapse ---

--- collapse ---

---
title: My eyes are not round
---

The third and fourth numbers in `ellipse` are the width and height of the eyes. 

**Tip:** If you make them the same, you will get round eyes.

--- /collapse ---


--- /task ---

--- save ---
## Add a mouth

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
A mouth is a great way of showing emotion. Will your character have a smile, frown, or something else? 
</div>
<div>
![Image showing a robot face as an example of a face with a mouth.](images/mask.png){:width="200px"}
</div>
</div>

--- task ---

Think about what kind of mouth your face needs. The simplest mouth would be a circle to look surprised. 

You could add two overlapping circles to create a smile or frown. Triangles or rectangles could be added for teeth. 

--- /task ---

--- task ---

Add code to your `draw()` function to add a mouth.

--- collapse ---

---
title: Create a mouth from overlapping circles
---

Set the `fill` colour for your mouth then draw an `ellipse`. Set the `fill` colour again, this time to match the face colour, then draw a second `ellipse`.

Change the `y` coordinate of the second `ellipse` to a slightly higher position for a smile or a slightly lower position for a frown. 

![The output area showing a smiling mouth.](images/smile.png)

--- code ---
---
language: python
filename: main.py - draw()
---

    fill(0, 0, 0)  # A black mouth
    ellipse(200, 240, 15, 15)
    fill(255, 165, 0)  # An orange face
    ellipse(200, 235, 15, 15)  # Higher circle

--- /code ---

![The output area showing a frowning mouth.](images/frown.png)

--- code ---
---
language: python
filename: main.py - draw()
---

    fill(0, 0, 0)  # A black mouth
    ellipse(200, 240, 15, 15)
    fill(255, 165, 0)  # An orange face
    ellipse(200, 245, 15, 15)  # Lower circle

--- /code ---

--- /collapse ---

--- collapse ---

---
title: Create a mouth using rectangles
---

Robots are often shown with `rectangle` shaped mouths. Sometimes `rectangle` and `ellipse` shapes are used together to create a grimace emoji or to add a face mask. 

![The output area showing a face with rectangle facemask.](images/rectangle-mask.png)

Add the code for a `rectangle`, then create a smaller `rectangle` within it. Change the `stroke` and `fill` colours to complement your theme. Add `ellipse` shapes if needed. 

**Tip:** Remember to put the `ellipse` shapes above the `rectangle` code if you want them to go behind the `rectangle` shapes. 

--- code ---
---
language: python
filename: main.py - draw()
---
    # Face mask
    no_fill()
    stroke(255, 255, 255)
    ellipse(150, 250, 30, 30)  # Left ear loop
    ellipse(250, 250, 30, 30)  # Right ear loop
    fill(255, 255, 255)
    no_stroke()
    rect(150, 230, 100, 40)  # Large white rectangle
    fill(108, 200, 206)
    rect(152, 235, 96, 30)  # Smaller blue rectangle

--- /code ---

--- /collapse ---

**Tip:** Add a `#Mouth` comment on the line before your mouth code to help you easily find the mouth code.

--- /task ---

--- task ---

**Choose:** You could also add multiple teeth to your mouth using `translate` to change the `x` coordinate after each tooth is drawn. 

--- collapse ---

---
title: Use a loop to add a row of teeth
---

Add code to create a `for` loop that repeats in order to create the number of teeth you need. 

![The output area showing a robot face with a row of rectangle teeth in different colours.](images/robot-teeth.png)

After each tooth has been drawn, add code to `translate()` it by the width of the tooth. 

You can also add code to change the colour of each tooth.

--- code ---
---
language: python
filename: main.py - draw()
---

    # Mouth
    fill(90, 110, 184)
    red = 90  # Starting amount of red
    green = 110  # Starting amount of green
    blue = 180  # Starting amount of blue
    for i in range (0,6):
        rect(100, 300, 33, 50)
        fill(red, green, blue)  # Uses variables to control the colour change each loop
        red = red+40
        blue = blue-30
        translate(33, 0)  # Move along the x coordinate by the width of a tooth


--- /code ---

--- /collapse ---

[[[processing-translation]]]

--- collapse ---

---
title: Use triangles to add fangs
---

Create a `rectangle` to use as the line of the mouth.

Add two `triangle` shapes to create the fangs. Change the `x` coordinates for each corner to position the fangs at opposite ends of the mouth line.

![The output area showing a vampire face with a rectangle mouth and two triangle teeth.](images/vampire.png)

--- code ---
---
language: python
filename: main.py - draw()
---
    # Mouth
    fill(0)
    rect(170, 260, 60, 5)  # Mouth line
    fill(0)
    triangle(170, 260, 180, 280, 190, 260)  # Left tooth
    triangle(210, 260, 220, 280, 230, 260)  # Right tooth
--- /code ---

--- /collapse ---

--- /task ---

--- task ---

**Debug:** You might find some bugs in your project that you need to fix. Here are some common bugs.

--- collapse ---

---
title: My overlapping shape goes outside the face
---

If you use two overlapping shapes to create a mouth, then you need to make sure the shape that is the same colour as the face doesn't go outside the face. If it does, then change the width or height of the shape so that it's small enough to fit inside the face. 

--- /collapse ---


--- collapse ---

---
title: I have too many teeth
---

Don't forget that `range()` creates a sequence of numbers starting from 0 not 1. This may make a difference to your code depending on how you have positioned your teeth. 

--- /collapse ---

--- /task ---

--- save ---
## Add more details

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Does your face or mask need more details to make it more interesting? 
</div>
<div>
![Image showing a face as an example with a headband accessory.](images/frida.png){:width="200px"}
</div>
</div>

--- task ---

You can use more shapes to add more features to your face or mask.

How can you give the face more personality? 

You could add:

+ A nose
+ Eyebrows
+ Ears 
+ Cheeks 
+ Highlights / catchlights
+ Whatever you like!

Just add the extra details that make sense for your drawing.

--- /task ---

--- task ---

You can make partly transparent colours by adding a fourth number to an RGB colour to give the **opacity**.

This code draws the overlapping highlights in the Kawaii fruit example:

--- code ---
---
language: python
filename: main.py - draw()
---

    # Highlights    
    fill(255, 255, 255, 70)  # 70 is transparency/opacity here    
    ellipse(170, 150, 35, 35)   
    ellipse(150, 160, 25, 25)    

--- /code ---

![Kawaii fruit image with highlights at different opacities: 30, 70, 150, 255. The lower value, 30, is more opaque and 255 is less opaque.](images/opacity.png)

--- /task ---

--- save ---
