# AI PROJECT ON MALARIA CELL DETECTOR

## INTRODUCTION:
Malaria is one of the most serious and widespread parasitic disease of humans. The clinical symptoms of malaria are manifested when parasites invade and multiply inside human red cells.
When a malaria-carrying mosquito bites a human host, the malaria parasite enters the bloodstream, multiplies in the liver cells, and is then released back into the bloodstream, where it infects and destroys red blood cells.

## PARASITIZED & UNINFECTED CELL

![image](https://user-images.githubusercontent.com/101791322/195879347-b23245da-8633-472b-ba52-4292bb1b9c75.png)


DATA SUMMARY:
This dataset contains 27560 png images of malaria Parasitized & uninfected cells.The images are grouped into 2 classes. There are 13780 images in each class.

### Classes
1. Parasitized
2. Uninfected

## TASK: BINARY CLASSIFICATION

## WE DEVICE THIS PROJECT INTO MULTIPLE STEPS
1. Importing library
2. Make subset of training,testing & validation
3. Data Processing [Prepare training and testing data]
4. Visualise Training Images
5. Build Arcitecture
6. Model Compilation
7. Training
8. Evaluation
9. Model saving
10. Prediction
11. Testing
12. Visualise Test Images

## LODING DATA / PREPARING DATA
* Make a subset of data into three parts train, test, and validation with the help of split folder library.

### DATA PROCESSING 
### [PREPARE TRAINING, TESTING, VALIDATION DATA]
* Training:   22069 images belonging to 2 classes.
* Validation: 2758 images belonging to 2 classes.
* Testing:    2760 images belonging to 2 classes.

## VISUALISE TRAINING IMAGES FROM BOTH CLASSES:

1. Parasitized:

![image](https://user-images.githubusercontent.com/101791322/195880026-24bb5666-3350-4a44-a87a-010d2f833624.png)

2. Uninfected:

![image](https://user-images.githubusercontent.com/101791322/195880245-a31efd3c-e6a9-44c2-8ffd-4597e7accd67.png)


## BUILD ARCHITECTURE:
Use VGG19 transfer learning technique to build a architecture for detect the malaria cell.
1. Total params: 20,074,562
2. Trainable params: 50,178
3. Non-trainable params: 20,024,384
* Use flatten layer to convert output into 1D array
* Use sigmoid activation function at last FCNN layer because only 2 classes are present.

MODEL COMPILATION & TRAINING & EVALUATION:
•	Use binary cross_entropy and adam optimaizer to compile a model
•	Train model on 50 epochs, and plot training, validation accuracy as well as loss and validation loss
•	After evaluating the model 
Train Accuracy & Loss: [0.2546966075897217, 0.9057048559188843]
Testing Accuracy&Loss [0.21056684851646423, 0.9217391014099121]


## MODEL SAVING:
* Save the model using h5

## PREDICTION & TESTING:
* Select the image from testing data for prediction after that convert
this image into array, and expand the diamension of image then
Select the maxarg and last making the prediction using if elase 
condition 

## VISUALISE SOME PREDICTION:

![image](https://user-images.githubusercontent.com/101791322/195880481-834a6ed9-b205-4474-83f7-8d203772213c.png)


### DEPLOY MODEL USING FLASK FRAMWORK

## LIBRARY USED: 
* Tensorflow
* Keras
* Matplotlib
* Glob
* Numpy
* Splifolder
* Open CV
* OS

## TOOL USED:
* Jupyter Notebook
* Pycharm 







