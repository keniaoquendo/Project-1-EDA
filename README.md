# Project-1-EDA - slide 1
By: Sally Anderson, Kenia Oquendo Berrios, Gwendolyn Lukman, and Jackie Rosales
Title: COVID-19 (and factors leading to) Deaths

# Introduction - slide 3
Topic: Healthcare on COVID 19
Analysis: External factors affecting death rates

# Datasets - slide 4
- Covid 19 deaths by sex and age
- Covid 19 vaccination rates
- 2022 state populations

# Cleaning the data - slide 5
- Filtering states (removing non-states such as Puerto Rico or Washington DC)
- Removing columns 
- Merging csv files together
- Grouping counties together under one state

# Reasearch Hypothesis
## Hypothesis 1 - slide 7
Null Hypothesis 1
- The percent of people who died of COVID-19 is NOT affected by the state population.
Alternate Hypothesis 1
- The percent of people who died of COVID-19 will be higher in more highly populated states than in less populated states.

* Our prediction is to reject the Null Hypothesis 1.
* Logic: If the population is densely concentrated, then death rates by percent of the population will be higher, because the population will have a higher rate of interaction with one another.

## Hypothesis 2 - slide 8
Null Hypothesis 2
- Vaccination does NOT contribute to a decrease in death risk.
Alterate Hypothesis 2
- Vaccination contributes to a decrease in death risk.
* Our prediction is to reject the Null Hypothesis 2.
* Logic: If a person is vaccinated, they are less likely to die, regardless of their state's population density.


## Analysis
## Population per state - slide 9
- show a bar chart showing the 2022 population estimate per state
- We can see that there is a lot of variance betweeen the state populations

## Deaths Per Region = Skewed Data - slide 10
- shows a pie chart of the COVID-19 deaths per region and Pnuemonia and COVID-19 Deaths Per region

## Calculating the Quartile and classifying states into different groups - slide 11-14
- We classified the states by their population sizes and came up with 4 groups (XL, large, medium and small)

## Death Comparisons - slide 15
- We chose certain states that represent each group and made a pie chart of showing the Total Deaths, COVID-19 Deaths and Pneumonia and COVID-19 Deaths

## Residents with Completed Primary Series - Slide 16-20
- We made a bar chart of each state by their groups (XL, large, medium, small) that includes, Total doses distributed, Total doses administered by jurisdiction, Residents 65+ with a completed primary series, Residents 18+ with a completed primary series, Residents 12+ with a completed primary series, Residents 5+ with a completed primary series
- We found that 
    - All states did not administer all doses that were distributed.
    - 65+ demographic had the lowest vaccination rates out of all the groups tested.
    - All states followed the same trend in vaccination totals: 5+ > 12+ > 18+ > 65+

## Correlation between Vaccination vs Total Deaths - slide 21
- The scatter plot shows the percent of total population with at least one dose vs total deaths.
- r-squared is 0.0069 which meant that there is no or very weak correlation between vaccination and death

## H1: Hypothesis Testing - slide 22
- Shows independent t-tests for 2022 Population Estimate vs COVID-19 Deaths
- p-value are as follows: 


## H2: Hypothesis Tesing - slide 23

