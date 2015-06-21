# cleaningdata

####Prerequsite: the phone data files need to be in the directory "UCI HAR Dataset" in the current working directory

####The run_analysis script reads in the activity labels from the file "activity_labels.txt" and gives proper column names
####As a second step the script reads in the list of data features from the file "features.txt"
####Next the script reads in the test data set and assigns proper column names
####after that the program reads in the training data set and assigns proper column names
####Then we assign the proper activity name to activity index and put together the phone data with the activities and subjects
####As next step the script assigns the proper activity name to activity index and put together the phone data with the ####activities and subjects
####Then we simply put the two part data sets (train,test) together
#### find the columns that represent either a calculated mean or standard 
#### deviation for any variable
#### filter out the required columns found with the command above, the number 
#### of the subject and activity name is included
#### with an aggregate function the mean value of each variable is calculeted for
#### each distinct subject and his activity
#### we delete the tidy data file to have a clear starting point
#### the result data is written in a tab separated text file sorted by the subject
#### index, only the necessary columns are written in the file, column 3,4 do not
#### carry any additional info

