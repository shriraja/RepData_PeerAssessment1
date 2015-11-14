---
title: 'Coursera Course Reproducible Research'
output: html_document
---

# Peer Assessment 1
<!--Steps performed
* Read the Activity Monitoring data 
* Converted the date variable type as Date
* Calculated the total number of steps per day using aggregate function
-->

## Histogram of total number of steps per day  
![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2-1.png) 

## Mean of the total number of steps taken per day  

```
## [1] 10766.19
```
## Median of the total number of steps taken per day

```
## [1] 10765
```
## Average Daily Activity Graph
![plot of chunk unnamed-chunk-5](figure/unnamed-chunk-5-1.png) 

## 5 Minute Interval that has Maximum Number of steps 

```
## [1] 835
```

## Total Number of missing values in the dataset

```
## [1] 2304
```

##Steps used for imputation
1. Iterate thru each row in activitydata
2. Check if the step value is NA
3. If it is true, then calculate the average for that interval for all the days and assign that value to it


## Histogram of total number of steps per day after imputation
![plot of chunk unnamed-chunk-9](figure/unnamed-chunk-9-1.png) 

## Mean of the total number of steps taken per day after imputation 

```
## [1] 10765.64
```
## Median of the total number of steps taken per day after imputation

```
## [1] 10762
```

## The Mean and Median values slightly differ before and after imputation but not much.
## The histogram pattern looks identical before and after the imputation and I didn't find much difference after imputing the data.


Weekdays Vs Weekend Graph comparison
---
![plot of chunk unnamed-chunk-12](figure/unnamed-chunk-12-1.png) 

## The pattern between weekday and weekend is different. The number of steps are high during weekend compare to weekday except between interval 750 and 1000.
