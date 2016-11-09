#Project Description

This file describes the data, the variables, and the work that has been performed to clean up the borrowed dataset of Samsung Galaxy S Smartphone data.


Description of data files
=========================

- 'features_info.txt': Shows information about the variables used on the feature vector.

- 'features.txt': List of all features.

- 'activity_labels.txt': Links the class labels with their activity name.

- 'train/X_train.txt': Training set.

- 'train/y_train.txt': Training labels.

- 'test/X_test.txt': Test set.

- 'test/y_test.txt': Test labels.

The following files are available for the train and test data. Their descriptions are equivalent.

- 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.

- 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.

- 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.

- 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.


#Procedures to create tidy data file
The following ‘train’ files of data from the directory \uci were read into R uci/train/X_train.txt uci/train/y_train.txt uci/train/subject_train.txt

These data were then combined together, by combining the columns together, to create a new data table (called “train”)

Then, the following ‘test’ files of data from the directory \uci were read into R uci/test/X_train.txt uci/test/y_train.txt uci/test/subject_train.txt

These data were also combined together, by combining the columns together, to create a new data table (called “test”).

The two data tables, “train” and “test”, were combined together by joining the rows of these tables together.

The column of subjects was labeled “subject”. The column of activities was labeled “activity”.

The activity numbers are replaced with their respective activity labels. The columns were labeled with their respective column names from the uci/features.txt file.

The tidy data set is this complete and saved as tidydata.csv in the \uci folder.

The R commands for tidying the data, extracting mean and standard deviation columns and calculating variable averages can be found in the following script.

Run_analysis.R
