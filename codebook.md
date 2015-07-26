## CodeBook
This document describes the variable definition used in <b>run_analysis.R</b> script to generates the tiday data (Tidy.txt).

## Data 
The data collected from the accelerometers from the Samsung Galaxy S smartphone.
A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The data for the project: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

## Input Data and variable assignment
The input data containts the following data files to assigned to a variable:
<ul>
  <li>featuresTrain stores data from X_train.txt</li>
  <li>activityTrain stored data from y_train.txt</li>
  <li>subjectTrain stored data Data from subject_train.txt</li>
  
  <li>featuresTest stored data from X_test.txt</li>
  <li>activityTest stored data from y_test.txt</li>
  
  <li>subjectTest stored data from subject_test.txt</li>
  <li>featureNames stored data from features.txt</li>
  <li></li>
  <li></li>

activity_labels.txt is read into activityLabels.
The subjects in training and test set data are merged to form subject.
The activities in training and test set data are merged to form activity.
The features of test and training are merged to form features.
The name of the features are set in features from featureNames.
features, activity and subject are merged to form completeData.
Indices of columns that contain std or mean, activity and subject are taken into requiredColumns .
extractedData is created with data from columns in requiredColumns.
Activity column in extractedData is updated with descriptive names of activities taken from activityLabels. Activity column is expressed as a factor variable.
Acronyms in variable names in extractedData, like 'Acc', 'Gyro', 'Mag', 't' and 'f' are replaced with descriptive labels such as 'Accelerometer', 'Gyroscpoe', 'Magnitude', 'Time' and 'Frequency'.
tidyData is created as a set with average for each activity and subject of extractedData. Entries in tidyData are ordered based on activity and subject.
Finally, the data in tidyData is written into Tidy.txt.
</ul>
