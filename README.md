# Lab 7: What did you say?
This lab, unlike the past, will be entirely new and different. As such, the grading will be simpler, the instructions VERY clear, and hopefully more fun to play around with and learn from. 

Given the newness of Transformer models into the field, instead of having some defined model and pattern for you to beat, you will follow two of the best tutorials that are currently available for building a sequence to sequence machine translation transformer. 

ACE Env:
* CPU: 2
* Memory: 32
* GPU: 1 (exclusive)


## Option 1: Keras Tutorial
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

## Option 2: Machine Learning Mastery
The overall tutorial can be found [here](https://machinelearningmastery.com/building-transformer-models-with-attention-crash-course-build-a-neural-machine-translator-in-12-days/). This tutorial is meant for a 12 day course, so please bear that in mind. They do provide links to a few sources for more data that may not be within the TF datasets if you wish to try other languages. 

Provide the same Deliverables as the Keras tutorial if you choose this one. 

## Option 3: PyLessons
Again, the full tutorial is [here](https://pylessons.com/transformers-introduction), but you can select the various sections you want on the right for deeper review. PyLessons is also very good about including tutorial videos, so feel free to watch those if you wish. 

Provide the same Deliverables as the Keras tutorial if you choose this one. 
