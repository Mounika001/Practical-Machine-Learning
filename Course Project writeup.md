# Practical-Machine-Learning
## Mounika Lakkadi
## Sunday, June 21, 2015

## Introduction

Using devices such as Jawbone Up, Nike FuelBand, and Fitbit it is now possible to collect a large amount of data about personal activity relatively inexpensively. These type of devices are part of the quantified self movement – a group of enthusiasts who take measurements about themselves regularly to improve their health, to find patterns in their behavior, or because they are tech geeks. One thing that people regularly do is quantify how much of a particular activity they do, but they rarely quantify how well they do it. In this project, your goal will be to use data from accelerometers on the belt, forearm, arm, and dumbell of 6 participants. They were asked to perform barbell lifts correctly and incorrectly in 5 different ways. More information is available from the website here

##Data 

The data for this project come from this source: http://groupware.les.inf.puc-rio.br/har.

The training data for this project are available here: 

https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv

The test data are available here: 

https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv

## Install necessary packages 

library(ggplot2)
library(caret)
library(randomForest)
library(rpart) 
library(rpart.plot) 
library(RColorBrewer) 
library(rattle) 
library(plyr)

## Set the working Directory

setwd("~/GitHub/PLM")

## Loading the data into R

## Replace missing values with NA

train<- read.csv("~/GitHub/PLM/pml-training.csv", na.strings=c("#DIV/0!"), row.names = 1)

# [1] 19622   159

test<- read.csv("~/GitHub/PLM/pml-testing.csv", na.strings=c("#DIV/0!"), row.names = 1)




