# Code Book

This code book describes the data fields in `tidy.txt` file.

## The Source Data

The tidy.txt data set is a combination of the following files:

1. x_test.txt
2. y_test.txt
3. subjext_text.txt
4. x_train.txt
5. y_train.txt
6. subject_train.txt
7. features.txt
8. activity_labels

## Transformation Steps
1. Merges the training and the test sets to create one data set.
  * Read in the data into the test and training sets
  * Bind the rows for each of the data sets together
  * Combine all of of the different columns together into one table
2. Extracts only the measurements on the mean and standard deviation for each measurement. 
  * Get the complete list of features
  * Filter to the required features
3. Uses descriptive activity names to name the activities in the data set
  * Read in the activity labels
  * Update the activity name
4. Appropriately labels the data set with descriptive variable names. 
  * Remove the brackets from the features columns
  * Convert the data into strings  
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
  * Melt the data to a unique row for each combination of subject and acitivites
  * Cast the data getting the mean value
  * Write the data out to a file

## Variables
There are **68 variables total**. 
The first two variables are used to aggregate the data by:

1. **subject** - Contains the ID of the subject who performed the activity, based on the following interval of IDs 
   - 1 - 30
2. **activity** - The activity identifier performed by the subject, based on the following list of identifiers
   - WALKING
   - WALKING_UPSTAIRS
   - WALKING_DOWNSTAIRS
   - SITTING
   - STANDING
   - LAYING

### The Full List of Variables

Index  | Variable Name
------ | -------------
1|subject
2|activity
3|tBodyAccmeanX
4|tBodyAccmeanY
5|tBodyAccmeanZ
6|tBodyAccstdX
7|tBodyAccstdY
8|tBodyAccstdZ
9|tGravityAccmeanX
10|tGravityAccmeanY
11|tGravityAccmeanZ
12|tGravityAccstdX
13|tGravityAccstdY
14|tGravityAccstdZ
15|tBodyAccJerkmeanX
16|tBodyAccJerkmeanY
17|tBodyAccJerkmeanZ
18|tBodyAccJerkstdX
19|tBodyAccJerkstdY
20|tBodyAccJerkstdZ
21|tBodyGyromeanX
22|tBodyGyromeanY
23|tBodyGyromeanZ
24|tBodyGyrostdX
25|tBodyGyrostdY
26|tBodyGyrostdZ
27|tBodyGyroJerkmeanX
28|tBodyGyroJerkmeanY
29|tBodyGyroJerkmeanZ
30|tBodyGyroJerkstdX
31|tBodyGyroJerkstdY
32|tBodyGyroJerkstdZ
33|tBodyAccMagmean
34|tBodyAccMagstd
35|tGravityAccMagmean
36|tGravityAccMagstd
37|tBodyAccJerkMagmean
38|tBodyAccJerkMagstd
39|tBodyGyroMagmean
40|tBodyGyroMagstd
41|tBodyGyroJerkMagmean
42|tBodyGyroJerkMagstd
43|fBodyAccmeanX
44|fBodyAccmeanY
45|fBodyAccmeanZ
46|fBodyAccstdX
47|fBodyAccstdY
48|fBodyAccstdZ
49|fBodyAccJerkmeanX
50|fBodyAccJerkmeanY
51|fBodyAccJerkmeanZ
52|fBodyAccJerkstdX
53|fBodyAccJerkstdY
54|fBodyAccJerkstdZ
55|fBodyGyromeanX
56|fBodyGyromeanY
57|fBodyGyromeanZ
58|fBodyGyrostdX
59|fBodyGyrostdY
60|fBodyGyrostdZ
61|fBodyAccMagmean
62|fBodyAccMagstd
63|fBodyBodyAccJerkMagmean
64|fBodyBodyAccJerkMagstd
65|fBodyBodyGyroMagmean
66|fBodyBodyGyroMagstd
67|fBodyBodyGyroJerkMagmean
68|fBodyBodyGyroJerkMagstd
