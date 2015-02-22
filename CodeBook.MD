## Getting and Cleaning Data Project


### Description
Additional information about the variables, data and transformations used in the course project for the Johns Hopkins Getting and Cleaning Data course.


### Section 1. Merge the training and the test sets to create one data set.

Data used was read into tables from these files:
- features.txt
- activity_labels.txt
- subject_train.txt
- x_train.txt
- y_train.txt
- subject_test.txt
- x_test.txt
- y_test.txt
Column names were assigned and merged to create one data set.

### Section 2. Extract only the measurements on the mean and standard deviation for each measurement. 

Create a logical vector that contains TRUE values for the Id mean and stdev columns and FALSE values for the others.
Only the necessary columns were kept.

### Section 3. Use descriptive activity names to name the activities in the data set

Merge data subset with the activityType table to include the descriptive activity names.

### Section 4. Appropriately label the data set with descriptive activity names.

Use gsub function for pattern replacement to clean up the data labels.

### Section 5. Create a second, independent tidy data set with the average of each variable for each activity and each subject. 

The script needs to produce only a data set with the average of each variable for each activity and subject.