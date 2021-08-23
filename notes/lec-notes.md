# Data 8: Foundations of Data Science

    University of California, Berkeley
    Instructors: David Wagner, Ani Adhikari
    daw@cs.berkeley.edu, adhikari@berkeley.edu
    Office Hours: -
    Lecture: Mon/Wed/Fri 10:00am-11:00am
    Author: Will Tholke

## Table of Contents

- [Data 8: Foundations of Data Science](#data-8-foundations-of-data-science)
  - [Table of Contents](#table-of-contents)
  - [Lecture 1, 08/25/21 (Wk1): Introduction](#lecture-1-082521-wk1-introduction)
    - [Subtitle #1](#subtitle-1)
  - [Lecture 2, 08/27/21 (Wk1): Cause and Effect](#lecture-2-082721-wk1-cause-and-effect)
    - [Subtitle #1](#subtitle-1-1)
  - [Lecture 3, 08/30/21 (Wk2): Tables](#lecture-3-083021-wk2-tables)
    - [Subtitle #1](#subtitle-1-2)
  - [Lecture 4, 09/01/21 (Wk2): Data Types](#lecture-4-090121-wk2-data-types)
    - [Subtitle #1](#subtitle-1-3)
  - [Lecture 5, 09/03/21 (Wk2): Building Tables](#lecture-5-090321-wk2-building-tables)
    - [Subtitle #1](#subtitle-1-4)
  - [Lecture 6, 09/08/21 (Wk3): Census](#lecture-6-090821-wk3-census)
    - [Subtitle #1](#subtitle-1-5)
  - [Lecture 7, 09/10/21 (Wk3): Charts](#lecture-7-091021-wk3-charts)
    - [Subtitle #1](#subtitle-1-6)
  - [Lecture 8, 09/13/21 (Wk4): Histograms](#lecture-8-091321-wk4-histograms)
    - [Subtitle #1](#subtitle-1-7)
  - [Lecture 9, 09/15/21 (Wk4): Functions](#lecture-9-091521-wk4-functions)
    - [Subtitle #1](#subtitle-1-8)
  - [Lecture 10, 09/17/21 (Wk4): Groups](#lecture-10-091721-wk4-groups)
    - [Subtitle #1](#subtitle-1-9)
  - [Lecture 11, 09/20/21 (Wk5): Joins](#lecture-11-092021-wk5-joins)
    - [Subtitle #1](#subtitle-1-10)
  - [Lecture 12, 09/22/21 (Wk5): Table Examples](#lecture-12-092221-wk5-table-examples)
    - [Subtitle #1](#subtitle-1-11)
  - [Lecture 13, 09/24/21 (Wk5): Iteration](#lecture-13-092421-wk5-iteration)
    - [Subtitle #1](#subtitle-1-12)
  - [Lecture 14, 09/27/21 (Wk6): Chance](#lecture-14-092721-wk6-chance)
    - [Subtitle #1](#subtitle-1-13)
  - [Lecture 15, 09/29/21 (Wk6): Sampling](#lecture-15-092921-wk6-sampling)
    - [Subtitle #1](#subtitle-1-14)
  - [Lecture 16, 10/01/21 (Wk6): Models](#lecture-16-100121-wk6-models)
    - [Subtitle #1](#subtitle-1-15)
  - [Lecture 17, 10/04/21 (Wk7): Comparing Distributions](#lecture-17-100421-wk7-comparing-distributions)
    - [Subtitle #1](#subtitle-1-16)
  - [Lecture 18, 10/06/21 (Wk7): Decisions and Uncertainty](#lecture-18-100621-wk7-decisions-and-uncertainty)
    - [Subtitle #1](#subtitle-1-17)
  - [Lecture 19, 10/08/21 (Wk7): A/B Testing](#lecture-19-100821-wk7-ab-testing)
    - [Subtitle #1](#subtitle-1-18)
  - [Lecture 20, 10/11/21 (Wk8): Causality](#lecture-20-101121-wk8-causality)
    - [Subtitle #1](#subtitle-1-19)
  - [Lecture 21, 10/13/21 (Wk8): Examples](#lecture-21-101321-wk8-examples)
    - [Subtitle #1](#subtitle-1-20)
  - [Lecture 22, 10/03/21 (Wk8): Midterm Review](#lecture-22-100321-wk8-midterm-review)
    - [Subtitle #1](#subtitle-1-21)
  - [Lecture 23, 10/18/21 (Wk9): Confidence Intervals](#lecture-23-101821-wk9-confidence-intervals)
    - [Subtitle #1](#subtitle-1-22)
  - [Lecture 24, 10/20/21 (Wk9): Interpreting Confidence](#lecture-24-102021-wk9-interpreting-confidence)
    - [Subtitle #1](#subtitle-1-23)
  - [Lecture 25, 10/22/21 (Wk9): Center and Spread](#lecture-25-102221-wk9-center-and-spread)
    - [Subtitle #1](#subtitle-1-24)
  - [Lecture 26, 10/25/21 (Wk10): The Normal Distribution](#lecture-26-102521-wk10-the-normal-distribution)
    - [Subtitle #1](#subtitle-1-25)
  - [Lecture 27, 10/27/21 (Wk10): Sample Means](#lecture-27-102721-wk10-sample-means)
    - [Subtitle #1](#subtitle-1-26)
  - [Lecture 28, 10/29/21 (Wk10): Designing Experiments](#lecture-28-102921-wk10-designing-experiments)
    - [Subtitle #1](#subtitle-1-27)
  - [Lecture 29, 11/01/21 (Wk11): Correlation](#lecture-29-110121-wk11-correlation)
    - [Subtitle #1](#subtitle-1-28)
  - [Lecture 30, 11/03/21 (Wk11): Linear Regression (and it's my birthday!)](#lecture-30-110321-wk11-linear-regression-and-its-my-birthday)
    - [Subtitle #1](#subtitle-1-29)
  - [Lecture 31, 11/05/21 (Wk11): Least Squares](#lecture-31-110521-wk11-least-squares)
    - [Subtitle #1](#subtitle-1-30)
  - [Lecture 32, 11/08/21 (Wk12): Residuals](#lecture-32-110821-wk12-residuals)
    - [Subtitle #1](#subtitle-1-31)
  - [Lecture 33, 11/10/21 (Wk12): Regression Inference](#lecture-33-111021-wk12-regression-inference)
    - [Subtitle #1](#subtitle-1-32)
  - [Lecture 34, 11/12/21 (Wk12): Privacy](#lecture-34-111221-wk12-privacy)
    - [Subtitle #1](#subtitle-1-33)
  - [Lecture 35, 11/15/21 (Wk13): Classification](#lecture-35-111521-wk13-classification)
    - [Subtitle #1](#subtitle-1-34)
  - [Lecture 36, 11/17/21 (Wk13): Classifiers](#lecture-36-111721-wk13-classifiers)
    - [Subtitle #1](#subtitle-1-35)
  - [Lecture 37, 11/19/21 (Wk13): Decisions](#lecture-37-111921-wk13-decisions)
    - [Subtitle #1](#subtitle-1-36)
  - [Lecture 38, 11/22/21 (Wk14): TBA](#lecture-38-112221-wk14-tba)
    - [Subtitle #1](#subtitle-1-37)
  - [Lecture 39, 11/29/21 (Wk15): TBA](#lecture-39-112921-wk15-tba)
    - [Subtitle #1](#subtitle-1-38)
  - [Lecture 40, 12/03/21 (Wk15): Conclusion](#lecture-40-120321-wk15-conclusion)
    - [Subtitle #1](#subtitle-1-39)


## Lecture 1, 08/25/21 (Wk1): Introduction

### Subtitle #1
  
-

## Lecture 2, 08/27/21 (Wk1): Cause and Effect

### Subtitle #1
  
-

## Lecture 3, 08/30/21 (Wk2): Tables

### Subtitle #1
  
-

## Lecture 4, 09/01/21 (Wk2): Data Types

### Subtitle #1
  
-

## Lecture 5, 09/03/21 (Wk2): Building Tables

### Subtitle #1
  
-

## Lecture 6, 09/08/21 (Wk3): Census

### Subtitle #1
  
-

## Lecture 7, 09/10/21 (Wk3): Charts

### Subtitle #1
  
-

## Lecture 8, 09/13/21 (Wk4): Histograms

### Subtitle #1
  
-

## Lecture 9, 09/15/21 (Wk4): Functions

### Subtitle #1
  
-

## Lecture 10, 09/17/21 (Wk4): Groups

### Subtitle #1
  
-

## Lecture 11, 09/20/21 (Wk5): Joins

### Subtitle #1
  
-

## Lecture 12, 09/22/21 (Wk5): Table Examples

### Subtitle #1
  
-

## Lecture 13, 09/24/21 (Wk5): Iteration

### Subtitle #1
  
-

## Lecture 14, 09/27/21 (Wk6): Chance

### Subtitle #1
  
-

## Lecture 15, 09/29/21 (Wk6): Sampling

### Subtitle #1
  
-

## Lecture 16, 10/01/21 (Wk6): Models

### Subtitle #1
  
-

## Lecture 17, 10/04/21 (Wk7): Comparing Distributions

### Subtitle #1
  
-

## Lecture 18, 10/06/21 (Wk7): Decisions and Uncertainty

### Subtitle #1
  
-

## Lecture 19, 10/08/21 (Wk7): A/B Testing

### Subtitle #1
  
-

## Lecture 20, 10/11/21 (Wk8): Causality

### Subtitle #1
  
-

## Lecture 21, 10/13/21 (Wk8): Examples

### Subtitle #1
  
-

## Lecture 22, 10/03/21 (Wk8): Midterm Review

### Subtitle #1
  
-

## Lecture 23, 10/18/21 (Wk9): Confidence Intervals

### Subtitle #1
  
-e

## Lecture 24, 10/20/21 (Wk9): Interpreting Confidence

### Subtitle #1
  
-e

## Lecture 25, 10/22/21 (Wk9): Center and Spread

### Subtitle #1
  
-e

## Lecture 26, 10/25/21 (Wk10): The Normal Distribution

### Subtitle #1
  
-e

## Lecture 27, 10/27/21 (Wk10): Sample Means

### Subtitle #1
  
-e

## Lecture 28, 10/29/21 (Wk10): Designing Experiments

### Subtitle #1
  
-e

## Lecture 29, 11/01/21 (Wk11): Correlation

### Subtitle #1
  
-

## Lecture 30, 11/03/21 (Wk11): Linear Regression (and it's my birthday!)

### Subtitle #1
  
-

## Lecture 31, 11/05/21 (Wk11): Least Squares

### Subtitle #1
  
-

## Lecture 32, 11/08/21 (Wk12): Residuals

### Subtitle #1
  
-

## Lecture 33, 11/10/21 (Wk12): Regression Inference

### Subtitle #1
  
-

## Lecture 34, 11/12/21 (Wk12): Privacy

### Subtitle #1
  
-

## Lecture 35, 11/15/21 (Wk13): Classification

### Subtitle #1
  
-

## Lecture 36, 11/17/21 (Wk13): Classifiers

### Subtitle #1
  
-

## Lecture 37, 11/19/21 (Wk13): Decisions

### Subtitle #1
  
-

## Lecture 38, 11/22/21 (Wk14): TBA

### Subtitle #1
  
-

## Lecture 39, 11/29/21 (Wk15): TBA

### Subtitle #1
  
-

## Lecture 40, 12/03/21 (Wk15): Conclusion

### Subtitle #1
  
*Note:* Final exam on Monday, 12/13/21 @ 8:00am-11:00am
-
