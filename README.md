# Human-Activity-Regonition
Human Activity Recognition (HAR) using smartphones dataset and an LSTM RNN. Classifying the type of movement amongst six categories(multi-class classification).<br>
Six-Categories:<br>

1.WALKING,
2.WALKING_UPSTAIRS,
3.WALKING_DOWNSTAIRS,
4.SITTING,
5.STANDING,
6.LAYING.<br>
**About Data:**
This dataset is collected from 30 persons, performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone.<br>
-Accelerometer readings are divided into total acceleration and body acceleration readings, which has x,y and z components each.<br>
-Gyroscope readings are the measure of angular velocities which has x,y and z components.<br>
-Pre-processing accelerometer and gyroscope readings using noise filters.<br>
-Splitting data into fixed windows of 2.56 seconds (128 data points) with 50% overlap.Splitting of accelerometer data into gravitational (total) and body motion components
**Train and Test Split**
1.The dataset was split into train (70%) and test (30%) sets based on data for subjects, e.g. 21 Persons data for train and 9 persons data for test.<br>
2.Each data-point corresponds to one of the six-activities
3.7352 train and 2947 test samples
**Note**
-There are three main signal types in the raw data: total acceleration, body acceleration, and body gyroscope. Each has 3 axises of data. This means that there are a total of nine variables for each time step.

-One row of data has (128 * 9), or 1,152 elements.

Data All the data is present at https://archive.ics.uci.edu/ml/machine-learning-databases/00240/UCI%20HAR%20Dataset.zip
