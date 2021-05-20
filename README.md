# Human Activity Recognition using smart-phones

**Description:-**
This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying.<br/>This dataset is collected from 30 persons(referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.

**How to use:-**
* The HAR_EDA.ipynb contains all the analysis done on the complete data, so use it for getting complete insight of the data.
* All classical machine learning models are implemented in HAR_PREDICTION_MODELS.ipynb using proper feature engineered features.
* HAR_LSTM.ipynb contains the predicitions using LSTM deep learning models.

**All of the conclusions & proper comparisons between models performances can be seen in ipynb notebooks.**

**Problem-Statement:**
Human Activity Recognition (HAR) using smartphones dataset and an LSTM RNN. Classifying the type of movement amongst six categories(multi-class classification).

**Six-Categories:**
 
* WALKING,
* WALKING_UPSTAIRS,
* WALKING_DOWNSTAIRS,
* SITTING,
* STANDING,
* LAYING.


**Data:**
* All the data is present in 'UCI_HAR_dataset/' folder in present working directory.Link: https://archive.ics.uci.edu/ml/machine-learning-databases/00240/UCI%20HAR%20Dataset.zip
     - Feature names are present in 'UCI_HAR_dataset/features.txt'
     - ___Train Data___
         - 'UCI_HAR_dataset/train/X_train.txt'
         - 'UCI_HAR_dataset/train/subject_train.txt'
         - 'UCI_HAR_dataset/train/y_train.txt'
     - ___Test Data___
         - 'UCI_HAR_dataset/test/X_test.txt'
         - 'UCI_HAR_dataset/test/subject_test.txt'
         - 'UCI_HAR_dataset/test/y_test.txt'

* Accelerometer readings are divided into total acceleration and body acceleration readings, which has x,y and z components each.
* Gyroscope readings are the measure of angular velocities which has x,y and z components.
* Pre-processing accelerometer and gyroscope readings using noise filters.
* Splitting data into fixed windows of 2.56 seconds (128 data points) with 50% overlap.Splitting of accelerometer data into gravitational (total) and body motion components

**Train and Test Split:-**

* The dataset was split into train (70%) and test (30%) sets based on data for subjects, e.g. 21 Persons data for train and 9 persons data for test.
* Each data-point corresponds to one of the six-activities
* 7352 train and 2947 test samples
