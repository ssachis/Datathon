# Datathon

Dataset used in this competition was RVL-CDIP ( https://www.kaggle.com/datasets/pdavpoojan/the-rvlcdip-dataset-test ) 
# ABOUT DATASET
For this competition, a part of RVL-CDIP dataset was used. It contained overall 16 classes with 1000 images per class.
Different classes were as follows -
letter
form
email
handwritten
advertisement
scientific report
scientific publication
specification
file folder
news article
budget
invoice
presentation
questionnaire
resume
memo

# Preprocessing 
1. A csv file was provided mapping the image name with respect to their class label. 
2. We made seperate folders per class. 
3. Images were moved to their respective class folder using shutil.
4. Then these images were extracted one by one, resized, converted to numpy arrays and normalized by dividing them with 255 to scale them in 0-1 range.
5. Labels were encoded using One Hot Encoding.

# Model 
We made a Sequential model having 3 convolutional layers following 4 dense layers having activation function as Relu and one output layer with activation function as softmax, maxpooling set as (2,2) and dropout rate as 0.1.

# Future Work
We can use OCR a computer vision technique for detecting and interpreting text in the images and classifying them accordingly.
