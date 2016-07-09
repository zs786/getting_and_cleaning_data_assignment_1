Course Project

Overview

The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project. You will be required to submit: 1) a tidy data set as described below, 2) a link to a Github repository with your script for performing the analysis, and 3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.

One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Here are the data for the project:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
You should create one R script called run_analysis.R that does the following.

Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive variable names.
Creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Good luck!

Evaluation Checklist

Tidy Data Set

From Question: Please upload a tidy data set according to the instructions in the project description. Please upload your data set as a separate file (do not cut and paste a dataset directly into the text box, as this may cause errors saving your submission).

From Evaluation: Has the student submitted a tidy data set?

Second Data Set

From Question: Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Github Repo with Required Scripts

From Question: Please submit a link to a Github repo with the code for performing your analysis. The code should have a file run_analysis.R in the main directory that can be run as long as the Samsung data is in your working directory. The output should be the tidy data set you submitted for part 1.

From Evaluation: Did the student submit a Github repo with the required scripts?

Code Book

From Overview: A code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md.

From Evaluation: Please submit a code book that modifies and updates the codebooks available to you with the data to indicate all the variables and summaries you calculated, along with units, and any other relevant information.

README

From Overview: You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.

From Question: You should include a README.md in the repo describing how the script works.

From Evaluation: I was able to follow the README in the directory that explained what the analysis files did.

Data Analysis Explanation

For 1st tiny data set:

Read data sets and combine them
Read subjects and combine them
Read data labels and combine them
Read features list
Subset only only std and mean features from list
Perform same subset on data set
Rename features to be more human readable
Read activity list
Rename activities to be more human readable
Rename data labels with activity name
Merge data, subjects, and labels to single tiny data set
Write tiny data set to file
For 2nd tiny data set: average of measurement for activity and subject

Prepare empty data set of appropriate length for
Loop through subjects, then subloop through activities
For each activity in a subject, get the full list of measurements
Calculate the mean of each of these activities
Place the means in subsequent columns of the subject/activity row
Write second tiny data set to file