How to run this project:

1. Unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder with "data".
2. Move the folder "Dataset" and the run_analysis.R script in the current working directory.
3. In R studio(or other R IDE) run source("run_analysis.R") command.
4. You will find two output files are generated in the current working directory:
        merged_data.txt (7.9 Mb): it contains a data frame called cleanedData with 10299*68 dimension.
        means_data.txt (220 Kb): it contains a data frame called result with 180*68 dimension.
5. use data <- read.table("means_data.txt") command in RStudio to read the file. Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.
