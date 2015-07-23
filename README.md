Getting and Cleaning Data
Author: Dr Shuhaida Mohamed Shuhidan

This is a repository for any and all code written for the Getting and Cleaning Data Coursera course through Johns Hopkins University to explains how all of the scripts work and how they are connected.

The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. 

Documents to submit: 
1) a tidy data set as described below, 
2) a link to a Github repository with your script for performing the analysis 
3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. 
4) a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.  


Course Project

Step 1

(find all project-related materials in the UCI HAR Dataset directory, however, copies of the important files have been put into this main directory to fulfill the submission requirement)

Unzip the source (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) into a folder on your local drive, say C:\Users\yourname\Documents\R\

Step 2

Put run_analysis.R into C:\Users\yourname\Documents\R\UCI HAR Dataset\

Step 3

In RStudio: setwd("C:\\Users\\yourname\\Documents\\R\\UCI HAR Dataset\\"), followed by: source("run_analysis.R")

run_analysis.R does the following;
Task 1. Merges the training and the test sets to create one data set.
Task 2. Extracts only the measurements on the mean and standard deviation for each measurement. 
Task 3. Uses descriptive activity names to name the activities in the data set
Task 4. Appropriately labels the data set with descriptive variable names. 
Task 5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Step 4

Use data <- read.table("data_set_with_the_averages.txt") to read the data. It is 180x68 because there are 30 subjects and 6 activities, thus "for each activity and each subject" means 30 * 6 = 180 rows. Note that the provided R script has no assumptions on numbers of records, only on locations of files.

