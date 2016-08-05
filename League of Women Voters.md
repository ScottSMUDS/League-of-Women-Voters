---
title: "League of Women Voters Analysis"
author: "Marvin Scott"
date: "August 1, 2016"
output: html_document
keep_md : TRUE
---

### **LW Voters analysis**



```{r setup, include=TRUE}
library(dplyr)


setwd("C:/Users/mscott4/Documents/LW Voters/")

lwv<- read.csv("LW Data.csv", header =  TRUE , sep =  ",")
##row count
nrow (lwv)
#top 20 records
head(lwv, 20)
#analysis
str(lwv)
#count of each voter.category
tapply(lwv$Voter.Category, lwv$Voter.Category, length)

```

### **Conclusion**

  The League of Women Voters need to determine the cause and effect experiment for Young Hispanic voters.This category of voters based on previous elections are less likely to participate in voter elections. By analyzing the provided dataset we can determine if the sample is a correct representaion of the Young Hispanic voters. 
  Based on the data reviewed,it was found that out of the 531736 total voters, only 41739 were Young Hispanics, merely between 7 and 8 percentage of the entire dataset. This raises questions on deriving a true cause and effect to this treatment group as the data does not reflect a correct representation of the experiment. 
  