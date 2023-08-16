## Train the model

Imagine teaching a friend how to differentiate between two types of fruits, let's say apples and bananas, by showing them pictures. At first, they might get confused, especially if they've never seen these fruits before. But as you keep showing them more pictures and correcting their mistakes, they start getting the hang of it. After a while, they can correctly identify apples and bananas on their own.

Training a machine learning model is kind of like this process, but with a computer instead of a friend. For your classifier, we want to determine 'hotdogs' and 'not hotdogs', so we need to define these two groups to the model, then provide lots of examples of each.

--- task ---

Select **Add new label** and create a label for the `hotdog` class.
![](images/add_hotdog.png)

**Repeat** this step to create a second label for the `nothotdog` class.

--- /task ---

--- task ---

We have collected two image sets for training your new machine learning model here (Click the plus sign to expand the collapses here):

[[[hotdog-train]]]

[[[not-hotdog-train]]]

Look through the training data and **choose several images of hotdogs and several images of other things** from the data. The more images of each type you pick, the more accurate your model will be. 

--- /task ---

--- task ---

Drag and drop your chosen images into the relevant class (`hotdog` or `nothotdog`).
![](images/hotdog_classes.png)

--- collapse ---
---
title: Adding training images with Drag & Drop
---

To 'drag and drop' images into your classes easily, you can set up the windows on your screen side-by-side by clicking on and dragging the tab you are working on to one side of the screen:
![Image showing two windows side by side on a computer screen. On the left are several images of hotdogs, on the right is a window showing a machine learning model's classes page](images/splitscreen.png)

Once you have set your screen up like this, you can simply just click on the training images you want to use and drag them into the right class, then release the mouse button:

![](images/dragdrop.gif)

--- /collapse ---

--- /task ---

--- task ---

Select **Back to project**.
![](images/back_to_project.png)

--- /task ---

--- task ---

Next, select **Learn & Test**.

![](images/learn_test.png)


Your model is now ready to be trained. 

--- /task ---

--- task ---

Select **Train new machine learning model**.
![](images/train_new.png)

You will have to wait a moment while the model trains.

--- /task ---

### Testing your model

Now that you have trained your model, it is time to test it to see how successful it is.  
Some data has been kept aside to use as test data.

When we want a computer program to learn a specific task, we give it a set of data to learn from. This set of data is called `training data`. It's like the exercises in your textbook that come with answers. You use these exercises to practise and understand the topic.

Once the program has learned from the training data, we need to check how well it has understood the task. To do this, we give it a new set of data it hasn't seen before, called `testing data`. This is similar to the questions on a quiz or test at school. The questions on the test aren't the exact ones you practised with, but they're about the same topic.

**Why Keep Them Separate?**
If we use the same data for both training and testing, it's like giving you a maths test with the exact same questions you practised with. You might get all the answers right, but it doesn't show if you understand the topic broadly. It only shows that you know those specific questions.

Similarly, if we test the computer program with the same data it trained on, we can't be sure if it has learned the task broadly or if it just "remembers" that specific data. By using different data for testing, we can get a better idea of how well the program can handle new, unseen situations.

So, it's essential to keep training and testing data separate to ensure that the computer program can perform the task accurately in various situations, not just the ones it has seen before.


To see how successful your model is at classifying the test data, test your model with some of the images:

--- task ---

Drag and drop an image into the link box (next to the Test with www button):

![](images/test_with_www.png)

--- collapse ---
---
title: Adding a test image without drag and drop
---

Alternatively, you can:

+ Right-click on an image
+ Select Copy image address
+ Paste the image address into the link box

--- /collapse ---

**You can find the testing images here:**

[[[hotdog-test]]]

[[[nothotdog-test]]]

--- /task ---

--- task ---

Click the **Test with www** button to test your model.

--- /task ---


--- task ---

Once you have tested a few of the images, answer the following questions in your **blueprint**:

1. Describe the results of your testing. How accurate was the model? 
2. Why do you think the prediction is sometimes  wrong?
3. How could you improve the accuracy of the model?

--- /task ---

### Bias and data

When we teach a computer to recognise different things, like dogs and cats, we need to give it lots of examples to learn from. These examples are called **training data**.

If we use a training dataset that contains mostly small dogs and large cats, this does not accurately represent the real world as there are also large dogs and small cats. If the data used to train the model is not representative of what you're trying to model,the prediction which your model makes won't be either.

This is called **bias**, which means the computer is favouring one thing over another. We can fix this by using a more diverse training dataset that includes different sizes and breeds of dogs and cats. By doing this, we can help the computer learn to recognise the features that distinguish each type of animal, rather than just relying on the size of the training examples.

<p style='border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;'>
By using more diverse and representative training data, we can help ensure that the computer makes accurate and fair predictions when it encounters new examples. This can make the computer more useful and reliable for different applications, from sorting pet adoption photos to assisting veterinarians in diagnosing animal health issues.
</p>

Let's start making your machine learning application in Scratch and think about what it will do!