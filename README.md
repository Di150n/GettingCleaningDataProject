# Getting and Cleaning Data - Course Project

This is the repository for the course project of the "Getting and Cleaning Data" course at Coursera.  

## Project Summary

The goal of this project is to create a tidy data set that can be used later to analyze the results of the experiments which were captured in the [Human Activity Recognition Using Smartphones] (http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) study.

The `run_analysis.R` script will run on the [data] (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) and it will complete the following steps to transform the data into more useful format to be analyzed later.

 1. Merges the training and the test sets to create one data set.
 2. Extracts only the measurements on the mean and standard deviation for each measurement. 
 3. Uses descriptive activity names to name the activities in the data set
 4. Appropriately labels the data set with descriptive variable names. 
 5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Repository Content

This repository contains the following files:

 - `run_analysis.R` - This script is used to download the source file, build up and perform the analysis on the required sample data.
 - `tidy.txt` - This is the final output from the `run_analysis.R` script.  It contains a cleansed version of the sample data.
 - `CodeBook.md` - Contains the definitions of each of the columns in `tidy.txt` file.

## About the `run_analysis.R` script

 - If the library `reshape2` is not installed, the `run_analysis.R` script will install it.
 - Also, the script will download the zip file if it does not exist already.