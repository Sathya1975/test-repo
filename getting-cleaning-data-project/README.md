## Getting and Cleaning Data Project
#----------------------------------------

# Sathyanarayanan Shanmugavelu

Repo for the submission of the course project for the Johns Hopkins Getting and Cleaning Data course.


## Overview
#----------------------------------------

This project serves to demonstrate the collection and cleaning of a tidy data set that can be used for subsequent analysis. A full description of the data used in this project can be found at The UCI Machine Learning Repository (http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

The source data for this project can be found here.(https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)


## Description of the Script (run_analysis.R)
#---------------------------------------------

# a. cleanup (the directory);

# b. fetch and unzip the data set;

# b.1 create data sub-directory if necessary
# b.2 download original data if necessary (skip if exists already as it takes time)
# b.3 unzip and creates dataSetDir if necessary

# c. read the data sets

# c.1 subjects IDs
# c.1 activities codes
# c.2 measurements

# d. merge datasets vertically, adding rows but keeping the same columns

# d.1 subjects
# d.2 activity codes
# d.3 measurements

# e. read feature and activity labels

# e.1 read as-is
# e.2 add column names and check

# f. renames columns of the merged measurement dataset with the feature labels

# g. filter the merged dataset to keep names with mean() or std() in them

# g.1 select the columns to keep
# g.2 subset by keeping the columns
# g.3. remove the parenthesis from the names

# h. add Subject and Activity columns in front

# i. add activity labels to the merged dataset

# j. aggregate and calculate the mean by subject and activity

# k. save the tidy dataset in data (tidy.txt)

# l. verify data


## Project Summary
#----------------------------------------

The following is a summary description of the project instructions

You should create one R script called run_analysis.R that does the following. 1. Merges the training and the test sets to create one data set. 2. Extracts only the measurements on the mean and standard deviation for each measurement. 3. Uses descriptive activity names to name the activities in the data set 4. Appropriately labels the data set with descriptive activity names. 5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject.


## Additional Information
#----------------------------------------
Additional information about the variables, data and transformations can be found in the CodeBook.MD file.
