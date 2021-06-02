#  Sentiment Analysis for KFC Menu Optimization using Python  

As we known the KFC restaurant is very popular in thailand , many
people can get to be fat due to the fact that fried product has a huge
calories and high amount of fat percentage more over the sodium that
is not good for our health if it was consumed with a high number.

The objectives of the study were to investigate of amount
nutrition. How many peoples should eats depend on how the body uses
them. The results to suggest to calculate the optimal of nutrition
require per day to good healthy for the regular people.

> Sentiment Analysis is the field of study that analyzes people's opinions, sentiments, evaluations, attitudes, and emotions from written languages. (Liu 2012)

## Contents

<!-- TOC -->

- [Problem and Descriptions](#problem-and-descriptions)
- [Survey Papers](#survey-paper)
- [Input Data](#input-data)
- [Objective](#objective)
- [Contrain](#contrain)
- [Algorithms Matching Methods](#algorithms-matching-methods)
- [Demonstrations](#demonstrations)
- [Conclusion](#conclusion)

<!-- /TOC -->

## Problem and Descriptions

- Number of overweight people is raising 13percent every year.
- Many menu set are difficult to predict calories.
- Almost are having big calories.
- No any consumer suggestion.
- Cholesteral and Sodium contain are noticeable.

## Survey Paper

This survey paper was created in google form, collecting data from student and teacher in SIIT faculty, Thailand.
The collected data are the sentimental score of each menu in Thai KFC menu.

- https://docs.google.com/forms/d/e/1FAIpQLSf3LA0RNB0qItKCIvT_czDyL9eEXB8RKUqcob9S3buDcSHr7g/viewform


## Input Data
Xij = information of each menu                             [ i for data group , j for number of menu ]
- X1j = name of menu
- X2j = Calories of menu
- X3j = Fats of menu
- X4j = Carbs of menu
- X5j = Proteins of menu
- X6j = Sodium of menu
- X7j = Cholesteral of menu
- X8j = Score of menu [ Satisfaction score ] restaurants

Ti = Target macro nutrients data
- T2 = Target Calories
- T3 = Target Fats(g)
- T4 = Target Carbs(g)
- T5 = Target Proteins(g)
- T6 = Target Sodium(g)
- T7= Target Cholesterols(mg)

## Objective
maximize Satisfaction
- max( z = sum(X8j) )

Minimize macro nutrition Error
- maximize  , z1 = sum( X_8j ) 
- minimize , z2 = abs( T2-sum(X_1j) )
- minimize , z3 = abs( T3-sum(X_2j) )
- minimize , z4 = abs( T4-sum(X_3j) )
- minimize , z5 = abs( T5-sum(X_4j) )
- minimize , z6 = abs( T6-sum(X_5j) )
- minimize , z7 = abs( T1-sum(X_6j) )

## Contrain
- Total error < 10 percentage
- Calories error < 20percentage
- Fat error < 20percentage
- Protein error < 20percentage
- Carbs error < 20percentage
- Cholesteral error < 20percentage

Difference
- Target value - Macro in Menu
- Positive = still have to consume
- Negative = have to eliminate menu

Macro error
- Absolute percent of Difference
Showing if these menu have error in target or not .

## Algorithms Matching Methods
- Random menu

## Demonstrations
Demonstrations (4example cases)
- A = Male 21years old, 175cm, 70kg, active level = 2
- B = Male 21years old, 175cm, 75kg, active level = 4
- C = Female 21years old, 158cm, 48kg, active level = 2
- D = Female 21years old, 158cm, 48kg, active level = 4

## Conclusion
- KFC menu have variaty menu with variaty of nutritient ratio.
- Sodium is the most factor that having a huge error
- Recommend to combine some low sodium menu to each meal
- Recommend KFC company to release new menu “low sodium Fried Chicken” or any healthy choice menu.
- Moreover, nutrients informations should be given to customers whatever restaurant is it.
