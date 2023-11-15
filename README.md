# Project-1-EDA
## Vaccination Rates and COVID-19 Deaths

## Introduction

## Reasearch Hypothesis
### Null Hypothesis 1: The percent of people who died of COVID-19 is NOT affected by the state population.
### Alternate Hypothesis 1: The percent of people who died of COVID-19 will be higher in more highly populated states than in less populated states.

* Our prediction is to reject the Null Hypothesis 1.
* Logic: If the population is densely concentrated, then death rates by percent of the population will be higher, because the population will have a higher rate of interaction with one another.

### Null Hypothesis 2: Vaccination does NOT contribute to a decrease in death risk.
### Alterate Hypothesis 2: Vaccination contributes to a decrease in death risk.
* Our prediction is to reject the Null Hypothesis 2.
* Logic: If a person is vaccinated, they are less likely to die, regardless of their state's population density.

## Datasets
* deaths per state
* states  pop
* vax per state

## Process
### Collect data
* Clean
* Merge
* Analyze

## Analysis
### H1
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


