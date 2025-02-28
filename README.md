# Getting and Cleaning Data Course Project

The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. Required submitions are: 1) a tidy data set as described below, 2) a link to a Github repository with your script for performing the analysis, and 3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.

One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained <a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">here</a>:

The data for the project is located <a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">here</a>.

# To get the tidy data:
1. Open R Program (I used RStudio)
2. Set WD to desired directory
3. run source("run_analysis.R") with provided script
4. In R console, view tidyDataAVG   OR open created text file "tidy-UCI-HAR-dataset-average.txt"



The script called run_analysis.R does the following.

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names.
5.  From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

output from run_analysis.R creates two files, one called tidy-UCI-HAR-dataset.txt which satisfies #3 & #4 and one called tidy-UCI-HAR-dataset-average.txt which satisfies #5 above.

The dataset is considered 'tidy' because:
1. Each row contains one observation
2. Each variable is split out into its own column and contains only one variable
3. Changed names to be user-friendly
4. Consolidated important datapoints on to a single table (merged with no duplicates)
