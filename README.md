# Project-1-EDA 
By: Sally Anderson, Kenia Oquendo Berrios, Gwendolyn Lukman, and Jackie Rosales
Title: COVID-19 (and factors leading to) Deaths

# Introduction
Topic: Healthcare on COVID 19
Analysis: External factors affecting death rates

# Datasets
- Covid 19 deaths by sex and age
- Covid 19 vaccination rates
- 2022 state populations

# Cleaning the data
- Filtering states (removing non-states such as Puerto Rico or Washington DC)
- Removing columns 
- Merging csv files together
- Grouping counties together under one state

# Reasearch Hypothesis
## Hypothesis 1
Null Hypothesis 1
- The percent of people who died of COVID-19 is NOT affected by the state population.
Alternate Hypothesis 1
- The percent of people who died of COVID-19 will be higher in more highly populated states than in less populated states.

* Our prediction is to reject the Null Hypothesis 1.
* Logic: If the population is densely concentrated, then death rates by percent of the population will be higher, because the population will have a higher rate of interaction with one another.

## Hypothesis 2
Null Hypothesis 2
- Vaccination does NOT contribute to a decrease in death risk.
Alterate Hypothesis 2
- Vaccination contributes to a decrease in death risk.
* Our prediction is to reject the Null Hypothesis 2.
* Logic: If a person is vaccinated, they are less likely to die, regardless of their state's population density.


## Analysis
### H1
* What is the population per state?
- show a bar chart showing the 2022 population estimate per state


* How many people died of covid per state? 
    * Show deaths per state visual. 
        - Break into regions (each graph has states in that region) 
        - 4 or 5 graphs in one slide, instead of all states on one graph
    * Is this sample size normally distributed?
    * Show histogram
    * stats analysis
    * What were our limitations from these datasets?
        - All sexes vs male/female
        - Ages??
        - Multiple conditions can skew data (pneumonia)

* What is the population of each state?
    * Show population per state visual? 
        - Break into regions (each graph has states in that region) 
        - 4 or 5 graphs in one slide, instead of all states on one graph
    * Is this sample size normally distributed?
    * Show histogram
    * stats analysis

* What is the correlation of the deaths vs population?
    * Show independent t-test of deaths per state vs population per state
    * Show overlapping histogram/population
    * What is the p-value?
    * Do we reject or fail to reject Null Hypothesis 1?

### H2
* How many people were vaccinated per state?
    * Show total vax per state visual
        - Break into regions (each graph has states in that region) 
        - 4 or 5 graphs in one slide, instead of all states on one graph
    * Show demographics
        - Vax per age differences
    * Is this sample size normally distributed?
    * Show histogram
    * stats analysis

* Use the data set of deaths per state from H1

* What is the correlation of the vax vs deaths?
    * Show scatter plot of vax per deaths, with linear regression r-value.
    * Show independent t-test of vax per state vs deaths per state.
    * Show overlapping histogram/population1 and population2
    * What is the p-value?
    * Do we reject or fail to reject Null Hypothesis 2?

### Summary of findings
* H1?
* H2?
* Highlight limitations of each data set.
    - deaths per state
    - pop per state
    - vax per state
* Future works

### References


