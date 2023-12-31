# Project-1
## Vaccination and COVID-19 Deaths
#### By: Sally Anderson, Kenia Oquendo Berrios, Gwendolyn Lukman, and Jackie Rosales


# Introduction 
* Topic: Healthcare 
* Analysis: Factors affecting COVID-19 death rates

The subject of this analysis is healthcare - specifically, COVID-19 death rates.  The chosen factors for hypothesis testing is if population density affects COVID-19 death rate, and if vaccination rates affect COVID-19 death rates. The data was collected from the U.S. Census, U.S. Department of Health & Human Services (HHS), and Centers for Disease Control and Prevention (CDC). 
- Time and scope were limiting factors:
    - Cummulative vaccination data, totaling years 2020-2023
    - Only states were chosen - all other U.S. territories were removed from the dataset
    - All sexes were analysized

Our analysis will highlight major trends, and if external factors influence COVID-19 death rates.


# Datasets
* HHS - Data.gov: Deaths involving COVID-19, pneumonia, and influenza reported to NCHS by sex, age group, and jurisdiction of occurrence.  
* U.S. Census - Census.gov: 2022 Population Estimate
* CDC - cdc.gov: COVID-19 vaccination rates

# Reasearch Hypothesis
## Hypothesis 1
- Null Hypothesis 1
    - The percent of people who died of COVID-19 is NOT affected by the state population.
- Alternate Hypothesis 1
    - The percent of people who died of COVID-19 will be higher in more highly populated states than in less populated states.

Our prediction is to reject the Null Hypothesis 1.
- Logic: If the population is densely concentrated, then death rates will be higher in more populated states because the population will have a higher rate of person-to-person interaction.

## Hypothesis 2
- Null Hypothesis 2
    - Vaccination does NOT contribute to a decrease in death risk.
- Alterate Hypothesis 2
    - Vaccination contributes to a decrease in death risk.

Our prediction is to reject the Null Hypothesis 2.
- Logic: If a person is vaccinated, then they are less likely to die from COVID-19.

# Analysis
## Cleaning and assembling data

### Population per state
The United States has a population that varies widely among the diffrent states. 
![image](images/Population_every_state.png)

The histogram of all states show highly skewed data.
![image](images/All_states_Pop_histogram.png)

### Calculating the Quartile and classifying states into different groups  
To help normalize the data, we classified the states by their population sizes and came up with 4 groups using interquartile analysis (XL, Large, Medium and Small). We removed the outlier states: NY, FL, TX, & CA. 

XL States (outliers) = population > 19,677,151 and < 39,029,342
- Accounts for 33% of total United States population

With the new dataset, with outliers states removed, we ran another interquartile analysis to create threshold for new datasets for the rest of the states:

Large States (Q3 - top 75% of data) = population < 19,677,151 and > 6,944,739
- Accounts for 35% of total United States population
- States: MA, NJ, PA, IL, MI, OH, GA, NC, TN, VA, AZ, WA

Medium States (Q2 - 50% of data) = population < 6,944,739 and > 1,816,125
- Accounts for 28% of total United States population
- States: CT, IN, IA, MN, MO, WI, AL, AR, KS, KY, LA, MD, MS, NE, OK, SC, CO, ID, NV, NM, OR, UT

Small States (Q1 - lowest 25% of data) = population < 1,816,125
- Accounts for 4% of total United States population
- States: ME, NH, RI, VT, DE, ND, SD, WV, AK, HI, MT, WY

## Death Comparisons 
We arbitrarily chose states to represent each group, showing the Total Deaths, COVID-19 Deaths, and Pneumonia and COVID-19 Deaths. 
- XL state: New York
- L state: Pennsylvania
- M state: Connecticut
- S state: Maine
![image](images/death_comp.PNG)
- The blue region shows the total of all deaths, due to any reason. The green region represents death due to multiple conditions (Pneumonia and COVID-19). The orange region represent death due to COVID-19. 
- The XL states had roughly 10% of the total deaths be due to COVID, while the large and medium state groups ranged from 7-9%, and the small states having roughly 5%. 
- We thought it was interesting the XL states still carry the higher percentage death rate while they make up 33% of the population as opposed to the large state group, which contains 35% of the population. This may be explaned by the fact that the XL states have more densely compacted communities.
- We considered multiple conditions and how it may raise the potential for death. We predicted the death rates would be overall higher among those with multiple conditions at time of death versus exclusively COVID-19. Specifically, we looked at the deaths of Pneumonia and COVID-19 versus those with just COVID-19. However, the pie charts reject our prediction and show that the percentage of multiple conditions did not make as big of an impact, with percentages ranging from 3% in the XL populated states, to 1% in the smaller populated states.

## Residents with Completed Primary Series
We made a bar chart of each state by their groups (XL, Large, Medium, Small) that includes, Total doses distributed, Total doses administered by jurisdiction, 
Residents 65+ with a completed primary series, Residents 18+ with a completed primary series, Residents 12+ with a completed primary series, Residents 5+ with a completed primary series
![image](images/XL_dose_bar.png)
![image](images/large_doses_bar.png)
![image](images/large_doses_bar.png)
![image](images/small_doses_bar.png)

Trends:
- 65+ demographic had the lowest vaccination rates out of all the groups.
    - We predicted this would be the highest because they were considered the highest risk group for death. 
    - We are unsure about why this was the case since each state targeted this demographic heavily.
- All states followed the same trend in vaccination totals: 5+ > 12+ > 18+ > 65+
    - Possible explanation: 
        - School age children (5+ & 12+ groups) were required to be vaccinated before going back to school
        - 18+ group wanted to get back to regular life faster (and possibly less fearful of adverse effects from the vaccine)
        - 18+ group may have been required by their workplace to be vaccinated before returning to work in person

## Doses per State
Total doses distributed vs Total doses administered by jurisdiction
 - XL state: New York
- L state: Pennsylvania
- M state: Connecticut
- S state: Maine
 ![image](images/doses.PNG)
  Trend: All states did not administer all doses that were distributed by the U.S. government.

## H1: Hypothesis Testing
T-tests for “2022 Population Estimate” vs “COVID-19 Deaths”
- All p-values are far below p = 0.05: 

| Population vs COVID-19 Death | p-values |
|------------|---------|
| All states | 0.00000008308 | 
| XL | 0.00791821963 | 
| L | 0.00000000768 | 
| M   | 0.00000000001 | 
| S   | 0.00000067855 | 

Conclusion: 
- We REJECT Null Hypothesis 1: The amount of people who died of COVID-19 is NOT affected by the state population.
- We CANNOT REJECT Alternate Hypothesis 1: The amount of people who died of COVID-19 will be higher in more populated states than in less populated states.

## H2: Hypothesis Testing 
T-tests for “Residents with at least one dose” vs 
“COVID-19 Deaths”
- All p-values are far below p = 0.05: 

| Vaccination vs COVID-19 Death | p-values |
|------------|---------|
| All states | 0.00000025333 | 
| XL | 0.00820147030 | 
| L | 0.00000002761 | 
| M   | 0.00000000004 | 
| S   | 0.00000223341 | 

Conclusion: 
- We REJECT Null Hypothesis 2: Vaccination does NOT contribute to a decrease in the likelihood of death from COVID-19.
- We CANNOT REJECT Alternate Hypothesis 2: Vaccination contributes to a decrease in the likehood of deaths from COVID-19

# Summary of Findings
Major Trends:
* The XL states had roughly 10% of the total deaths be due to COVID, while the large and medium state groups ranged from 7-9%, and the small states having roughly 5%. 
* 65+ demographic had the lowest vaccination rates out of all the groups tested.
* All states followed the same trend in vaccination totals: 5+ > 12+ > 18+ > 65+
* All states did not administer all doses that were distributed.

Question 1: 
* What is the relationship between the amount of people who died of COVID-19 and the state population?

* Based on the data, we CANNOT REJECT the alternative hypothesis that says: The amount of people who died of COVID-19 will be higher in more populated states than in less populated states.

Question 2:
* What is the relationship between vaccination and its ability to protect from COVID-19 death? 

* Based on the data, we CANNOT REJECT the alternative hypothesis that says: Vaccination contributes to a decrease in the likelihood of death from COVID-19.

# Limitations and Future Works
* Limited to USA
* Cumulative data (year 2020 - 2023)
* Population data is only from latest 2022 Census data (does not account for population changes in 2023)

* Future works include analyzing additional data, such as gender, age, to see effects on death, and through time (years, months).

## Resources
1. HHS - Provisional COVID-19 Deaths by Sex and Age: https://catalog.data.gov/dataset/provisional-covid-19-death-counts-by-sex-age-and-state
2. Census - 2022 Population Estimate: https://www2.census.gov/programs-surveys/popest/datasets/2020-2022/state/totals/
3. CDC - COVID-19 vaccination rates: https://covid.cdc.gov/covid-data-tracker/#vaccinations_vacc-people-booster-percent-pop5 



