## What next?

Now it's time to upgrade your project to make it more fun or interesting!

You could:
+ Add a new costume to the sprite to replace the Scratch cat:
[[[scratch3-add-costumes-to-a-sprite]]] 

+ Add a new backdrop to your project:
[[[generic-scratch3-backdrop-from-library]]]

+ Add sounds to your project:
[[[generic-scratch3-sound-from-library]]]

+ Make your application do something depending on whether the model says 'hotdog or nothotdog':

--- collapse ---
---
title: Making changes based on the label
---

Use an `if/else`{:class="block3control"} block with an equals operator to check if the label for the input is 'hotdog'. **If** it is, do something. Otherwise, do something else. This could be `change costume to []`{:class="block3looks"} or `play sound []`{:class="block3sound"}, or anything you like!

![Image showing a yellow if/else block with a green equals operator block inside it. Inside that is a block which determines which label the model has selected based on input.](images/label_if.png)

--- /collapse ---

+ Make your application do something based on how confident it is about its prediction:

--- collapse ---
---
title: Making changes based on the confidence of the model
---

Use the `recognise image (backdrop image) confidence` block with size and volume controls, or have something happen if the confidence is above or below a certain level:

![A list of blocks. A set volume block, a set size block and an if block, all have a block which determines the confidence of the model inserted into their variable ports.](images/confidence_if.png)

--- /collapse ---

**This was just the warm up!** Now that you know how to build a text classification application that can detect hotdogs, what do **you** want to make? 

In the next stage of the Experience AI challenge, you'll get to use the skills you've learnt in this project to create something totally cool and unique using Scratch and Machine Learning! [Click here](rpf.io/xaichallenge) to take the next exciting step in creating your own Artificial Intelligence app!