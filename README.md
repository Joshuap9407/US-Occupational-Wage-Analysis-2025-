US Occupational Wage Analysis (2025)

Analyzed the BLS datasets for 2025 to understand how wages vary across different occupations and states. 

Research Questions
1. What are the highest-paying jobs in each state?
2. What is the average wage by state?

Methodology
- Filtered to state-level rows using AREA_TYPE == 2
- Converted wage columns to numeric using pd.to_numeric() to handle BLS values marked as *
- Grouped by state to extract the top paying occupations and averages wages of each state

Key Findings
- Medical occupations tend to be the highest earners regardless of the state's average wage. For example, Nebraska and Missouri had low average wages, however, when analyzing the highest-paying jobs in each state, they had the highest paying occupations out of the entire US.
- Despite most urban states like New York having the highest average wages, there are outliers like Florida which has a lower average wage than a rural state like Alaska
- The difference between the highest and lowest paying state, DC and Mississippi, was $33,202
- Although DC had the highest average wage ($94,947), it had the lowest top-paying position (Family Medicine Physicians, $321,950). This suggests DC's high average is driven by many well-paying government occupations rather than a small number of extreme earners. On the contrary, a state like Nebraska has a low average 
  wage but the highest paying occupation (Cardiologists, $627,390) in the country.
  
Limitations and What I'd Improve
- The data analyzed was only from 2025, therefore, if more data is added from other years, the results may differ
- Medical specialities cause a skew in the data so it would be interesting to analyze how the results would change if medical specialities are excluded
- Alongside the average wage, there needs to be a cost of living adjustment for each state as we know states like New Jersey have a high cost of living

Tools: python, pandas, plotly

Data Source: BLS Occupational Employment and Wage Statistics (OEWS), May 2025
https://www.bls.gov/oes/tables.htm




