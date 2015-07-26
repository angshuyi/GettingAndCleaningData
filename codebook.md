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
  <li>activityLabels stored data from activity_labels.txt</li>
  <li>subject is the combination of subjects in training and test data </li>
  <li>activity is the combination of activities in training and test data</li>
  <li>features is the combination of feature test and trainiing data</li>
  <li>featureNames is the features properties</li>
  <li>CompleteData is the combination of features, activity and subject</li>
  <li>Index columns that contains std or mean and ignore case sensative and assigned to requiredColumns</li>
  <li>create extractedData from columns from requiredColumns</li>
  <li>Update descriptive names for activity for Activity column in <b>extractedData</b></li>
  <li>Acronyms in extractedData like 'Mag', 'f' and 't' being replaced with descriptive labels 'Magnitude', 'Frequency' and 'Time'</li>
  <li>tidyData is created based on activity and subjects from extractedData</li>
  <li>outoput data from tidyData was writte to a file named Tidy.txt</li>
</ul>

## Output File
Tidy.txt is a a space-delimited value file with header which contains the variable names that are easy to understand. The data in the files are values of mean and standard deviation.
