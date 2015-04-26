
==================================================================
Course Project Description - Analysis of average mean and standard deviations in Human Activity Recognition
Using Smartphones Dataset
Version 1.0
==================================================================

The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project.

The following are required to be submitted:
1. a tidy data set as described below
2. a link to a Github repository with your script for performing the analysis, and
3. a code book called CodeBook.md that describes the variables, data, and any work performed to clean up the data. 
4. a README.md in the repo with your scripts that explains how the script works. 

One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Here are the data for the project: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

The project expects the creation of one R script called run_analysis.R that does the following.
•	Merges the training and the test sets to create one data set.
•	Extracts only the measurements on the mean and standard deviation for each measurement. 
•	Uses descriptive activity names to name the activities in the data set
•	Appropriately labels the data set with descriptive activity names. 
•	Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 

What you find in this repository
•	CodeBook.md: information about raw and tidy data set and elaboration made to transform them
•	LICENSE.txt: license terms for data text and code
•	README.md: this file
•	run_analysis.R: R script to transform raw data set in a tidy one

How to create the tidy data set
1.	Ensure that you have an active internet connection to download data from the external site
2. 	open a R console and set the working directory to the repository root (use setwd())
3.	source ("run_analysis.R") script (it requires the plyr package)
4.           After execution of script, the file tidydata.txt should be present in your working directory.

The process executed by the run_anaysis.R script
1.	Creates a data directory, downloads the data archive and unzips the data for use	
2.	Reads all the input files: training data; test data; feature names and activity codes 
3.           Merges training and test sets to create one data set.
4.	Extracts only the measurements on the mean and standard deviation for each measurement.
5.	Names the activities in the data set with descriptive activity names
6.	Appropriately labels the data set with descriptive variable names.
7.	From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
8.	Writes the independant tidy data into a tidydata.txt file

Release Notes
•	The script has been tested for a windows installation of R only

The Data Set used for the project - Human Activity Recognition Using Smartphones Dataset Version 1.0
	For more information about this dataset contact: activityrecognition@smartlab.ws

	The dataset includes the following files:
	- 'README.txt'
	- 'features_info.txt': Shows information about the variables used on the feature vector.
	- 'features.txt': List of all features.
	- 'activity_labels.txt': Links the class labels with their activity name.
	- 'train/X_train.txt': Training set.
	- 'train/y_train.txt': Training labels.
	- 'test/X_test.txt': Test set.
	- 'test/y_test.txt': Test labels.
	- 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample.
	   Its range is from 1 to 30. 
	- 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis 
	   in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 
	   'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis. 
	- 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity
	   from the total acceleration. 
	- 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each
	   window sample. The units are radians/second. 

License:
	Use of this dataset in publications must be acknowledged by referencing the following publication [1] 

	[1] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity 
	Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop
	of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012

	This dataset is distributed AS-IS and no responsibility implied or explicit can be addressed to the authors or their 
	institutions for its use or misuse. Any commercial use is prohibited.

	Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, Davide Anguita. November 2012.

