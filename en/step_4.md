
## Make a Scratch application to classify images

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Your model is trained and ready to test, but to do that you need to create a scratch project that can allow your user to input images and classify the input as `hotdog` or `nothotdog`.
</div>
<div>
![Image showing a cat standing in front of a hotdog saying the confidence score of a machine learning model that it is indeed a hotdog](images/demo_shot.png){:width="300px"}
</div>
</div>


### **Your project will:**
+ Take audio input from the user
+ Use your trained ML model to classify sounds
+ Move a sprite on-screen based on the classification

--- task ---

On your [**project page**](https://machinelearningforkids.co.uk/#!/projects){:target="_blank"}, select **Make**:
![Image showing a button reading Make and the explanation 'Use the machine learning model you've trained to make a game or app, in Scratch, Python, or App Inventor'](images/make_button.png)

--- /task ---

--- task ---

On the next page, select Scratch 3
![](images/scratch3_button.png)

--- /task ---

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
A special fork of Scratch will open in a new tab. When it does, you will see an item in the left-hand menu with the same name as your machine learning project.

The new grey blocks you can see in that menu allow you to access your machine learning model from within your project:
</div>
<div>
![Image showing several Scratch block menus, with the final one being titled MusicWellness with the machine learning for kids logo](images/model_blocks_menu.png){:width="100px"}
</div>
</div>

--- collapse ---
---
title: Pro tip - Save your work!
---

This special version of Scratch allows you to access your machine learning model, as well as use the music database blocks - **if you try to open your project in another version of Scratch online it won’t work**. 

A hack you can use is to save your work to your computer often. Once you have the .sb3 file for your project saved you can open it again later, or on another computer:
+ Go to [rpf.io/mlscratch](rpf.io/mlscratch){:target="_blank"} to get to this special fork of Scratch 
+ Once Scratch opens choose File > Load from your Computer
+ Select your file in the window that appears to get back to where you left off

![Image showing the Scratch file menu with the Load from your computer option highlighted](images/load_menu.png)


Save your work as often as you can to make sure you don’t lose any progress!

--- /collapse ---

--- task ---

Add a `when green flag clicked`{:class="block3events"} block to your workspace. This is the script that will run the first time we start the project. 

```blocks3
when green flag clicked
```

--- /task ---

--- task ---

From the blue `Motion`{:class="block3motion"} menu, add a `set rotation style [left-right]`{:class="block3motion"} block to your script.

```blocks3
when green flag clicked
set rotation style [left-right]
```

--- /task ---



In the next step, you can customise the way your application looks by adding costumes and add some new features that activate depending on the classification of your input.

