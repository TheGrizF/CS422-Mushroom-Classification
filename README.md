# CS422-Mushroom-Classification
By: Michael Evans & Grant Fitch

This repository contains two notebooks:
CleaningData.ipynb is used to clean the original raw dataset provided by
the UC Irvinie Machine Learning Repository.  This dataset can be found in this repository at 
MushroomDataset/secondary_data.csv.  When ran it produces graphic analysis of the data, 
cleans and encodes the data and produces an encoding dictionary.
The end output of this notebook is the clean_mushroom_data.csv file to be used
for training the model.

Classify.ipynb handles the training, testing, and evaluating of our
gradient boosting classifier used to predict the edibility of mushrooms.  It will read in
the previously cleaned dataset stored as clean_mushroom_data.csv. 
This program uses k-fold cross validation to evaluate the best hyperparameter
for training the gbc on our clean mushroom data.  After training, the model
is then evaluated with testing producing accuracy, precision, recall, and f1 scores.

The MushroomDataset folder contains the original raw dataset, the expanded secondary dataset used
for this project, and several .txt files that can be used to decode the initial values of the raw 
data values.  This includes a key for colors, as well as other categorical features in the original dataset.
