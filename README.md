# cleaningdata


## read in the activity labels and give proper column names


## read in the list of data features


## read in the test data set and assign proper column names


## read in the training data set and assign proper column names


## assign the proper activity name to activity index

## put together the phone data with the activities and subjects


## assign the proper activity name to activity index

## put together the phone data with the activities and subjects


## simply put the two part data sets (train,test) together


## find the columns that represent either a calculated mean or standard 
## deviation for any variable


## filter out the required columns found with the command above, the number 
## of the subject and activity name is included


## with an aggregate function the mean value of each variable is calculeted for
## each distinct subject and his activity


## we delete the tidy data file to have a clear starting point
file.remove("tidy_data.txt")

## the result data is written in a tab separated text file sorted by the subject
## index, only the necessary columns are written in the file, column 3,4 do not
## carry any additional info
write.table(arrange(result_data[c(1,2,5:ncol(result_data))],Subject),"tidy_data.txt",sep="\t",row.names=FALSE)
