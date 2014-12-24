---
title: "lab 1 useful commands"
output: html_document
date: "Wednesday, December 24, 2014"
---
#### 1)read in table
```{r}
present=read.table("http://s3.amazonaws.com/assets.datacamp.com/course/dasi/present.txt")
```

#### 2)count the rows and columns
```{r}
size=dim(present)
```
#### 3)find the max value
```{r}
ind=which.max(present$boys+present$girls)
present$year[ind]
```
#### 4)directly compare the vectors
```{r}
com_result=present$boys>present$girls
com_result
```
#### 5)absolute value calculation
```{r}
present$year[which.max(present$boys-present$girls)]
```

