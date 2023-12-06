## Train the model

Imagine you're teaching a parrot to mimic certain words. You say "left", and you want the parrot to repeat "left". At first, the parrot might not get it correct, maybe it squawks or says something different. But if you keep repeating "left" to the parrot and reward it when it repeats the word correctly, eventually it will start saying "left" back to you. The same goes for "right", "up", and "down". After some time, whenever you say one of these words, the parrot will repeat it perfectly.

Training an audio classifier is a lot like teaching this parrot, but with a computer instead of a feathery friend. We want the computer to recognise the words 'left', 'right', 'up', and 'down'. So, we repeatedly "tell" the computer these words (in lots of training samples) and correct it if it gets them wrong. After a while, just like the parrot, the computer will be able to identify these words whenever it "hears" them.

--- task ---

Select **Add new label** and create a label for the `up` class.
![](images/add_up.png)


--- /task ---

--- task ---

**Repeat** the above step to create a label for each remaining class: `down`, `left`, and `right`.

![](images/all_classes.png)

--- /task ---

--- task ---

Inside the `up` class, click `Add example`. 

![Button that reads '+ add example'.](images/add_example.png)

--- /task ---

--- task ---

Click the microphone to record a sample of yourself (and anyone else you want!) saying `up`. 
**Note:** You can only record a maximum of 2 seconds in each sample.

![A pop-up window that says "Add example. Record an example of 'background noise'", with a small blue icon showing a microphone.](images/add_background_noise.png)

--- collapse ---
---
title: Some tips for recording your voice
---

Imagine you're teaching a new word to a friend from another country. Sometimes you might say the word slowly and clearly, and other times you might say it quickly or in your everyday speaking style. This helps your friend understand the word no matter how it's said. Recording your voice for the audio classifier is similar!

+ Find a quiet spot: Just like finding the best place to teach your friend the new word, pick a spot where there's no background noise. This helps the model process just your voice.

+ Speak clearly...but not always: Start by saying "left", "right", "up", and "down" very clearly. But also, mix it up! Sometimes say them quickly, or the way you'd say them in a regular conversation. This teaches the computer to classify the words even when they're not perfectly pronounced.

+ Hold the mic steady: If you're using a microphone or a phone, hold it steady, about a hand's length away from your mouth. A headset mic shouldn't touch your face when you speak. 

+ Not too loud, not too soft: Speak at a normal volume. Imagine you're chatting with your friend at the park – not too shouty, but not whispering secrets either.

+ Do a test run: Before diving in, record a short clip and listen to it. If you can understand yourself, the computer can probably process the data accurately too!

By giving the computer a mix of clear and everyday pronunciations, it'll be able to process real-world examples, no matter how you (or your users) say the words. (One of Google's voice assistant training datasets - called PRESTO - contains more than five hundred and fifty thousand conversations in six languages!)

--- /collapse ---

--- /task ---

--- task ---

**Record** lots of samples for each class. You must add **a minimum of eight samples in each class**, or you can't train your model. 

--- collapse ---
---
title: How many samples should I add?
---

Eight is the **very lowest** number of samples each class can have to create a working model. 

You should aim for **around 10-15 samples of each word**, but again - the more **training data** you add to your model at this stage, the more accurate it will be at classifying the words you say.


--- /collapse ---

--- /task ---

--- task ---

When you have enough samples in each class, select **Back to project**.
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

You will have to wait a few moments while the model trains - read the information below about testing while the model is processing!

--- /task ---

### Test your model

Now that you have trained your model, it is time to test it to see how successful it is.  

--- collapse ---
---
title: Training data vs. testing data
---

To train a machine learning model to classify a specific item, we provide it with a particular set of data called **training data**. This data set is similar to the exercises in a textbook that have answers; they help in understanding and practicing the topic.

After the model has processed the training data, it's essential to check the model's performance. For this, we input a new set of data known as **testing data**. Think of this as taking a quiz or test at school: the questions aren't identical to what you practiced, but they cover the same topic.

**Why keep them separate?**
If we use the same data for both training and testing, it's like giving you a maths test with the exact same questions you practised with. You might get all the answers right, but it doesn't show if you understand the topic broadly. It only shows that you know those specific questions.

Similarly, if we test the model with the same data it was trained on, we can't be sure if it has analysed enough data to make accurate predictions or if it has already classified that specific data during training. By using different data for testing, we can get a better idea of how well the model can classify **new** items of data.

So, it's essential to keep the training and testing data separate to make sure you get a realistic assessment of how the model performs. 

--- /collapse ---


Once the training is finished, see how successful your model is at classifying the test data. 

--- task ---

Click the `Start listening` button to test your machine learning model.
![Image that says 'Try making a sound to see how it is recognised based on your training' with two buttons beneath. A darker blue button reads 'start listening' and a light blue button reads 'stop listening'.](images/start_listening.png)

Say one of the words that you have trained the computer to classify: "up", "down", “left”, or “right”. If your machine learning model can correctly process it, it will show a prediction of what you said.

--- /task ---

--- task ---

If you’re not happy with how the model is working, go back to the **Train** page (by clicking **Back to project** and then **Train**) and add more examples to all the training classes. Try varying your speed and pronunciation, or get other people to add samples in their voice...or doing funny voices yourself!

--- /task ---

--- task ---

Once you have tested the model a few times, answer the following questions in your **Blueprint**:

1. Describe the results of your testing. How accurate was the model? 
2. Why do you think the prediction is sometimes wrong?
3. How could you improve the accuracy of the model?

--- /task ---

--- collapse ---
---
title: Bias and data
---

When we train a model to classify different things, like the words "yes" and "no", we need to give it lots of examples. These examples are called **training data**.

If we use a training data set that contains mostly loud "yes" and quiet "no" sounds, this does not accurately represent the real world as there are also quiet  "yes" and loud "no" sounds. If the training data is not representative of what you want to model, the model is more likely to output an incorrect prediction.

This is called **bias**, which means the model favours one thing over another. We can fix this by using a more diverse training data set that includes different volumes, tones, and emphasis of the "yes" and "no" sounds. By doing this, we can help the model identify the features that distinguish each word, rather than just relying on the volume of the sounds.

--- /collapse ---

<p style='border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;'>
Imagine you are making an app that identifies musical instruments by their sounds.
<br><br>
Now, think of ten instruments you could record for your training data. What if you only picked instruments common in a rock band, like guitars and drums? What happens when someone tries to identify the sound of a sitar or a didgeridoo? Have you considered both Western and non-Western instruments?
<br><br>
By using a broad and diverse set of instrument sounds in your training data to avoid <strong>bias</strong>, the app has a better chance at correctly classifying a wide range of instruments from all over the world. This ensures that the app is useful to music lovers everywhere, from a jazz club in New York to a traditional music festival in India.
</p>

Let's start making your machine learning application in Scratch and think about what it will do!
