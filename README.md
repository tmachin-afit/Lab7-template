# Lab 7: What did you say?
This lab, unlike the past, will be entirely new and different. As such, the grading will be simpler, the instructions VERY clear, and hopefully more fun to play around with and learn from. 

Given the newness of Transformer models into the field, instead of having some defined model and pattern for you to beat, you will follow two of the best tutorials that are currently available for building a sequence to sequence machine translation transformer. 

ACE Env:
* CPU: 2
* Memory: 32
* GPU: 1 (exclusive)


## Step 1: Keras Tutorial
https://www.tensorflow.org/text/tutorials/transformer

Yes, I know you can copy/pasta most of the code. That is not the point (see deliverables below). Follow the tutorial and create a single script that contains the various classes necessary to translate Portuguese to English. Compare your output to the final output from the tutorial. Make sure to comment anything you did differently than the tutorial (if you needed to change the layer sizes, etc) and why you did these changes.

### Tutorial Flow
#### Data Handling 

Follow the steps as described in the tutorial. Click the 'Toggle Code' blocks to get the full code. Make sure to download the TF Datasets, as it contains the necessary training and validation data for the language conversion. Test the dataset output so you can verify it actually does what you think and contains what you think it should. 

Add commments in this section comparing this process to the process followed for Lab6. Save your vacabulary files in the 'vocab' folder. 


### Define the components 
Create the individual components of the Transformer model, as defined in the tutorial. Add docstrings to each class so you can better reference it later. This is done using the triple quotation marks (""" """). Follow this process explicitly, as the methods are defined to be utilized by TF to actually do all of the cool things. 

Docstrings and getting it working

### Transformer
Compile your model, ensuring the layers and parameters are the same as the tutorial. 

### Training
For the training, make sure to include the Tensorboard callback so you can more easily visualize the process. Save the logs in the logs directory so I can verify as well. 

Comment in this section the total training time, as well as your thoughts on the process of training these models. 

### Inference
Complete the inference activities in the tutorial, and include the outputs as comments. 

### Deliverables
The key deliverables I will be checking for this step: 
* Comments requested in each part
* model saved in the model folder
* training logs
* vocabulary
* plots

## Step 2: Review additional tutorials
Once you have completed the Keras tutorial, take a little time (NOT TOO MUCH. DON'T DO THESE AS WELL UNLESS YOU REALLY REALLY WANT TO) and review these two other tutorials. Make sure you understand the steps they are taking, and comment on any key differences in approach. Remember, SKIM these. 

### Machine Learning Mastery 
The overall tutorial can be found [here](https://machinelearningmastery.com/building-transformer-models-with-attention-crash-course-build-a-neural-machine-translator-in-12-days/). This tutorial is meant for a 12 day course, so please bear that in mind. They do provide links to a few sources for more data that may not be within the TF datasets if you wish to try other languages. 

Comment on any key differences from the Keras tutorial.

### PyLessons
Again, the full tutorial is [here](https://pylessons.com/transformers-introduction), but you can select the various sections you want on the right for deeper review. PyLessons is also very good about including tutorial videos, so feel free to watch those if you wish. 

Comment on any key differences from the Keras tutorial. 

### Deliverables
Comment in your 'lab7.py' your responses to the above MLM and PyLessons tutorials. 

## Step 3: Now auf Deutsch
Now that you have a working Transformer that translates Protuguese to English, we want to make one that translates English to German. Please review the MLM tutorial [here](https://machinelearningmastery.com/training-the-transformer-model/) on training a model for English to German. Specificlaly, the Pickled dataset is retrieved from [here](https://github.com/Rishav09/Neural-Machine-Translation-System/tree/master).

For the following test inputs, provide your model output:
*This class really is pretty cool. 
*My name is <Student Name>
*The squirrels went skydiving, but missed their target. 

Comment on what your model might be doing well, or might be getting wrong. 

### Deliverables
Include the german model in the 'models' folder. 
Include the test output as comments. 
Include figures of the attention matrices of these phrases (if possible)
Include your comments on the model outputs
New Vocab file (as it will be different from your Portuguese file)

## BONUS:
BONUS POINTS!!! If you can train a model to translate from English to some fictional language (Preferrably a Tolkein language), and another model to translate back. 
