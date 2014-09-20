---
title: "Readme"
---

This readme will describe the requirements of run_analysis.R, how to run the file and load the outputted data back into R.  A description of the variables and their units and the transformations this script makes to the raw data is included in CookBook.md in this repo.

## Requirements

* R version 3.1.1
* Package plyr version 1.8.1
* Package reshape2 version 1.4
* The [raw data package](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) downloaded and unziped in the current working directory.

## How to run this script

1. Download run_analysis.R from github.

2. Download the dataset from (here)[https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip] and extract its contents to the same directory as run_analysis.R.  Do not change any folder names or file names.

3. Start an R console and set the working directory to where you downloaded the script and data set.

4. Run the following R commands to run the script.

```R
setwd("path to directory with script & data")
source("run_analysis.R")
```

## To view the data output

```R
data <- read.table("tidy_data.txt", header=TRUE, stringsAsFactors = FALSE)
head(data)
```