# Tunisian license plate recognition
Use two datasets to build a machine learning model that can recognize Tunisian licence plate

## Project overview
#### This project can divide into 4 steps
1. Build a machine learning model(CNN/VGG depends on which has better accuracy) that can recognize digit numbers from 0 to 9, and a special Tunisian letter in the middle of the licence plate
2.  
    * Use .xml file from dataset to locate the licence plate from pictures
    * Build another ML model taht can decate licence plate by itself(If I have time to do it) 
3. Split licence plate into different chunks and each chunk has one digit or one Tunisian letter
4. Apply trained ML model on to those letters and output the licence plate

## Dataset
* __File name:__ [LP](LP) | [LP_digit](LP_digit)
* __Source:__ [Link to LP folder source](https://www.kaggle.com/datasets/achrafkhazri/labeled-licence-plates-dataset) | [Link to LP_digit folder source](https://www.kaggle.com/datasets/khazri/tunisian-licence-plate)
* __Limitation:__ Some numbers in pictures been chopped are very hard to see, because of the resolution of the origional picture is too low.

## Data Perprocessing:
* Remove all pictures that their licence plates are not parallel to ground(ie. some pictures in the file are been rotated) 
* Remoce pictures that their licence plates are too small
* Remove pictures that are hard to see(low resolution)
* Use .xml file to chop pictures and only keep the licence plate part
* Restructure the LP file to make all pictures and .xml files under one single folder

## Link to Jupyter Notebook
* __Link to ML model:__ [Jupyter Notebook](Digit_recognize.ipynb)
* __Link to xml excract:__ [Jupyter Notebook(Not finished yet)]()
* __Link to split licence plates:__ [Jupyter Notebook(Not finished yet)]()

## Future Improvement
1. Instead using .xml file to get the licence plates from pictures, use another way tp get wher licence plates located in pictures.
2. <font color='red'> THINGS NEED TO BE ADDED HERE </font>
3. 

## How to run this project
1. __Install Required Libraries:__ `pip isntall numpy tensorflow opencv-python pillow`
2. __Clone from GitHub repo:__ `git clone https://github.com/NoBugInMyCode/Tunisian_license_plate_recognition.git`
3. __Run ML notebook:__ `python ML_model.ipynb`
4. __Run xml excract notebook:__
5. __Run split licence plate notebook:__
6. __Run predict function:__