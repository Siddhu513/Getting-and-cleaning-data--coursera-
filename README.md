Getting-and-Cleaning-Data-Week-4-Assignment
This repository containst the submission for the assignment for week 4 of Getting and Cleaning Data Coursera course.•First, download and unzip the data file into your R working directory.•Second, download the R source code into your R working directory.•Finally, execute R source code to generate tidy data file.

Data description
The variables in the data X are sensor signals measured with waist-mounted smartphone from 30 subjects. The variable in the data Y indicates activity type the subjects performed during recording.

Code explaination
The code combined training dataset and test dataset, and extracted partial variables to create another dataset with the averages of each variable for each activity.

New dataset
The new generated dataset contained variables calculated based on the mean and standard deviation. Each row of the dataset is an average of each activity type for all subjects.

The code was written based on the instruction of this assignment

The R script called run_analysis.R does the following. 1.Merges the training and the test sets to create one data set.2.Extracts only the measurements on the mean and standard deviation for each measurement. 3.Uses descriptive activity names to name the activities in the data set4.Appropriately labels the data set with descriptive variable names. 5.From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

In this project, data collected from the accelerometer and gyroscope of the Samsung Galaxy S smartphone was retrieved, worked with, and cleaned, to prepare a tidy data that can be used for later analysis.

This repository contains the following files:

README.md, this file, which provides an overview of the data set and how it was created. tidy_data.txt, which contains the data set. CodeBook.md, the code book, which describes the contents of the data set (data, variables and transformations used to generate the data). run_analysis.R, the R script that was used to create the data set (see the Creating the data set section below) Study design

The source data set that this project was based on was obtained from the Human Activity Recognition Using Smartphones Data Set

Creating the data set

The R script run_analysis.R can be used to create the data set. It retrieves the source data set and transforms it to produce the final data set by implementing the following steps (see the Code book for details, as well as the comments in the script itself):

Download and unzip source data if it doesn't exist. Read data. Merge the training and the test sets to create one data set. Extract only the measurements on the mean and standard deviation for each measurement. Use descriptive activity names to name the activities in the data set. Appropriately label the data set with descriptive variable names. Create a second, independent tidy set with the average of each variable for each activity and each subject. Write the data set to the tidy_data.txt file. The tidy_data.txt in this repository was created by running the run_analysis.R script using
R version 4.1.2 (2021-11-01)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows 10 x64 (build 22000)