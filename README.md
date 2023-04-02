# Healthcare-Ai

Deep Learning with PyTorch for Medical Image Analysis. Using Pytorch-Lightning to solve real world medical imaging tasks!


project: 01
# Pneumonia Classification 


* Pneumonia is a common infectious disease. In 2017 1.3 million people were diagnosed with pneumonia in United states.
* Research Says: About 1 million adults in the US seek care in a hospital due to pneumonia every year, and 50,000 die from this disease. than the age extremes, it is always a threat. Half of all non-immunocompromised adults hospitalized for severe pneumonia in the US are younger adults (18-57 years of age).


### What are the first warning signs of pneumonia?


- Early symptoms are similar to influenza symptoms: fever, a dry cough, headache, muscle pain, and weakness. Within a day or two, the symptoms typically get worse, with increasing cough, shortness of breath and muscle pain. There may be a high fever and there may be blueness of the lips.


### About the dataset:


- Data work
* We collected the images from the Kaggle dataset repository and we got 26684 images. In this we are using 24000 imgaes for the training the model and 2684 images for the validation
* Resize the imeage size : We have the images in 1024 * 1024 and we are resizing in 224 * 224


### Network Architechture:
- Restnet 
* change input channels from 3 to 1 
* change output dimensions from 1000 to 1 
* Loss function: BinaryCrossEntropy, Directly applied th logits (raw predictions)
* Negative Output = No Pneumonia
