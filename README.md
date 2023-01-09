# Project Title : "Music Preference Prediction Using Electroencephalogram (EEG) and Machine Learning Algorithm"

## Purpose and Brief Outcome
This project aims to predict music preference using electroencephalograms (EEG) and machine learning models. With a MUSE 2 EEG headband, 100 data (48 data for liked songs and 52 data for disliked songs) was collected and used to train machine learning models which will be able to classify whether someone is listening to a song that he/she likes or dislikes. With the help of EEG feature extraction method and PCA, the classification accuracy obtained are 100% (ANN), 87.63% (CNN), 100% (SVM) and 80.1% (Naive-Bayes).

## Contributers
1. Pang Tsz Tuen
2. Remy Zhang
3. Dhanush Kumar
4. Milena Markovich
5. Grace Quan
6. Pablo Palero

## Dependencies
* The project is developed using Jupyter Notebook with Python as the programming language.

## Prerequisites
* Project requires Python 3.11.0 to run.

## Installation steps for Jupyter
* Please click on <a herf = "https://docs.jupyter.org/en/latest/install/notebook-classic.html">Jupyter NoteBook</a> which contains instructions to install using IPython Kernal.
* Optional : Please click on <a herf = "https://docs.anaconda.com/anaconda/install/index.html">Anaconda </a> which contanins instructions to install Anaconda. 

## Usage
* Run the following code:

Open Anaconda Terminal: src/jupyter notebook EEG_Code.ipynb

* Select 'Kernal' then 'Restart and Run All'

* The images generated using the 256 PCS for the CNN model is stored inside Data/GeneratedImages

## Methodology and Conclusion
* Using a MUSE 2 EEG headband, a series of real-time brainwave data is collected from all group members, 
as well as external participants. The method proposed by Jordan J. Bird is then used to pre-process the raw EEG data and create a dataset which would yield meaningful results in the machine learning models.

* The pre-processing stage includes elimination of null values and unreasonable data, feature generation, splitting into training (80%) and testing (20%) sets, and feature scaling. After this step, principal component analysis is  performed to generate the top 256 PCs for feeding into the ANN, SVM and NB classifiers. 

* The 256 PCs are scaled to produce grayscale images to pass into the CNN model. 

* ANN Model and Non-Linear SVM
ANN model of the pre-processed data yields an accuracy of 100% on the test set without
overfitting. This accuracy is impossibly high, the reason might be the limited amount of
data points, as well as bias within subject selection and extremity of classifications as
possible causes for this.

* CNN Model
Two CNN models are used to analyze, first CNN model yields a training accuracy of 99.23% and a test set accuracy of 87.63%. The second CNN model follows the architecture in Jordan J. Bird’s research and is able to achieve an accuracy of 97.70% on the training set and an accuracy of 87.63% on the test set.

* Naive Bayes Classifier
Naive-Bayes classifier, yields an accuracy of 84.91% on the training set, and 80.10% on the test set

* To expand on this project, it is proposed that the use of transfer learning models,
such as the pre-trained VGG16 model


## Furture Applications of the Project
* Music therapy is an emerging discipline that integrates music, medicine, psychology, and other fields. Research in this field has made important contributions to psychological rehabilitation treatment of prenatal education, children's autism, Alzheimer's disease, and other health conditions. The emotional perception of humans is very important in social cognition and biological evolution; and music can be used as a stimulus to bring out these emotions in humans.

## Expected Output
* The percentage of accuracy for Train Set and Test Set for various models ANN, CNN, SVM & Nauve Bayes is calculated 


