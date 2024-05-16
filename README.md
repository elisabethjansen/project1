# Project 1 - Census Housing Exploratory Data Analysis 

Our objective within this project was to pull an analyze US Census data over multiple years and multiple variables to asses the question: 

How have housing trends, such as homeownership rates and rental affordability, changed over time across different demographics? 

### Data Source
All data was sourced using the US Census ACS5 API wrapper. Data was collected for 2019-2022 from all US zip codes. We identified 22 variables of interest across 4 categories using the data dictionary provided by the Census. 

## Analysis 
Each member of the team began with one analysis focus based on the initial question. Each focus lent itself to further questions and analysis after initial exploration into the topic. 

### Homeownership Trend Exploration
The key questions within this analysis were: 

How has home ownership rate changed over time? 
How has household income changed overtime? 

The initial exploration consited of generating a general statistical summary to understand data distribution, followed by an examination of the yearly distribution. 

Variables were identified and selected for analysis and analyzed for any existing relationships indicating how median household income could affect homeownership rate. 

Comparative analysis using a histogram showed distribution of homeownership rates across different zip codes and years. A linear regression model was used to understand and quantify the relationship between homeownership rates and median household income. 

The two analyses concluded that despite significant economic events between 2019 and 2022, the distribution remained similar, pointing to resilient homeownership trends. And additionally, while hypothesized that median household income is a major factor in homeownership, the analysis indicates a more complex relationship that varies across ZIP codes and time.

### Regional Exploration 

In this analysis 3 relationships of interest where tested on a national level (all US zip codes) using the 2022 census data. The relationships analyzed: 

Median gross rent vs population, poverty percentage vs population, poverty percentage vs median gross rent. 

A linear regression was compleded for each of the three relationships. The relationship indicating the highest r-value and lowest p-value was used for further analysis. 

The questions explored through further analysis are as follows: 

Do midwest zip codes display the same relationship of zip code population to median gross rent? How do the median rents of each state compare to each other? 

Can the same relationship be represented by comparing 3 states from differing region? 


Do independent state zip codes show the same relationship between zip code population and median gross rent as was seen in larger analyses? 

Scatter plots and linear regressions were completed for each regional set of data. All analyses indicated that we could rejec the null hypothesis of no relationship between zip code population and median gross rent. The only completed analysis where we failed to reject the null was in looking at Connecticut zip codes alone. 

This analysis lends itself well to further exploration to find other indicators of higher or lower median gross rent (ex. regional weather trends, diversity, etc.)

### Affordability trends and demographics
This exploration aimed to investigate the questions: 

How has the average rent to income ration changed form 2019-2022? How has the average owner cost to income ratio changed from 2019-2022? Do different Age groups experience similar trends in rent/income ratio? 

Analyses done on the above questions showed: 

Rent to income ratio is relatively statble from 2019 to 2021 as it hovers around 12% with a noticable decline in 2022 where the ratio drops to around 10%. 

Owner costs remained consistend over 2019 to 2022 with households spending, on average, about 25% of their income on ownership costs. 

Rent to income ratio by age group held consisted when looking at age ranges from under 25 to over 75 years of age, with each group showing a ratio of about .12. Similarly the ownership cost to income ratio by age group showed little to no variation. 

### Homeownership and affordability over time? 
This exploration aimed to investigate the question: what is the realtionship between median household income, median gross rent, median monthly owner costs, and race demographics? 

Analyses into each part of the above question showed: 

Consistently Rising Costs: Both ownership and rental costs have been rising, creating affordability challenges.

Income Growth: Median household incomes are increasing, which helps mitigate some of the affordability issues but may not be sufficient for all groups.

Racial Disparities: Significant trends in homeownership rates vary by race, highlighting disparities in access to homeownership that need attention.

The data initially souced spanned 4 years (2019-2022) this proved to be too short of a timeframe to find significant trends in homeownership. Data from 2014 was pulled to gain better insight into the question. 

Both short-term and long-term analyses show a strong upward trend in monthly ownership costs, indicating that owning a home is becoming more expensive over time. This trend is slightly more variable over the long term, suggesting fluctuations in economic conditions or housing policies.

Similar to ownership costs, median gross monthly rent costs have also been increasing consistently. This trend highlights the growing affordability challenges in the rental market, affecting those who may not be able to afford homeownership.


## References 

Data dictionary variables source https://api.census.gov/data/2021/acs/acs5/variables.html 