Overview
========
Script run_analysis.R  performs following steps: 

Step #1 - Merges the training and the test sets to create one data set.
Step #2 - Extracts only the measurements on the mean and standard deviation for each measurement. 
Step #3 - Use descriptive activity names to name the activities in the data set.
Step #4 - On the whole dataset, those columns with vague column names are corrected.
Step #5 - Generate a new dataset with all the average measures for each subject and activity type (30 subjects * 6 activities = 180 rows). 
          The output file is called tidy.txt, and uploaded.
          
Variables
=========
test.labels stores y_test.txt  (from test data) & assigns column name label
test.subjects stores subject_test.txt (from test data)& assigns column name subject
test.data stores X_test.txt data(from test data)  
train.labels stores y_train.txt  (from train data) & assigns column name label
train.subjects stores subject_train.txt (from train data)& assigns column name subject
train.data stores X_train.txt data(from train data)
data combines both test & train data in the format : subjects, labels, everything else
features stores features.txt by stripping leading & trailing white spaces
features.mean.std strips & retains only mean & std
data.mean.std stores only mean & std data
labels stores names of activities
descriptive.colnames stores only meaningful column names & features names by removing non-alphabetic characters & converting to lovercase
aggrgt.data stores the mean of each combination of subject & label


