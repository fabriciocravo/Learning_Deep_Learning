This course is called Practical Deep Learning for Coders

It can be found in https://course.fast.ai


Class 1 - Getting started 

It is simply an introduction to fast ai. It uses an example of creating a classifier to indify if a photo is either of a birth or not. 

Interesting Points:
    - There is a module called duckduckgo_search for automating searches in ddgs. I had to update the code as it appears their usage was depracated. One can use the constructor DDGS() to search text, images and others. The first argument of the object created by the DDGS() (ddgs in code) has methods like .image for which the first argument is the term to be searched. It also has a maximum value to avoid overloading the API.
    
    - There is a module called fastdownload for doawloading content from urls. It is used in the notbook from course one to dowload the images of birds to train the classifier 
    
    - The code has bad programming practices - (from fastai.vision.all import *) - does not allow me to keep track of where some of the functions come from. - Note for future self when using and developping MobsPy
    
    - Fastai - highly important - DataLoarders object. Used to store data for training neural nets. It needs the following for it's constructor: blocks - description of the problem, with the type of data or if it is or not a classification problem, 
   get_items - needs a function that returns the method of retreving the data. In this example, it takes get_image_files which takes the image files from a directory.
   splitter - spilts the data into training and validation set
   get_y - needs a function that returns the label of the image 
   item_tfms - methods to apply to data before training 
   
   - Needed to switch from GPU to CPU - I would expect the switch to be automatic with a warning for the user ....
   
   - Well mac loses again fastai does not support intel macs, lovely. I will run the next ones on the kaggle kernel


Class 2 - Deployment



