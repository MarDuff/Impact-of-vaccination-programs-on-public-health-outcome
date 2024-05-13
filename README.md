### Impact-of-vaccination-programs-on-public-health-outcome

#### INTRODUCTION

In today's world, life has been significantly affected while simultaneously having substantial challenges for our future and current generations due to the COVID-19 pandemic that has emerged and created a tremendous impact on public health. Having the ability to control the viral spread and mitigating its impact has become one of the top concerns for every country on the globe (J.R Zahar et al., 2022). One of the many approaches that were executed to manage the spread of infection through vaccination was the implementation of vaccination incentive programs and policy interventions. These strategies were vital in encouraging willing public participation in vaccination efforts and adhering to safety measures, the ultimate foundation for healthy communities(12 COVID-19 Vaccination Strategies for Your Community, 2022). Our project's primary goal is to assess these interventions' effectiveness using data analysis techniques. 

To accomplish this project, we will use a comprehensive data set that includes various metrics related to public health initiatives and outcomes during the pandemic. The dataset sourced from the CDC contains records detailing the number of administered vaccine doses per age group, per 100k pop, and other variables that influenced public health metrics. The key metrics we used for this report are: 

	State – Record of each state applicable to the tested parameters.

	Total Doses Distributed – Total recorded doses distributed per state during the sampling period.

	Doses Distributed per 100k Pop – The total number of distributed doses per 100k Pop to have a more comparable measure between large and smaller states.

	COVID–19 Mitigation Policy – A record of states implementing COVID-19 mitigation bills/laws. 

	Lottery – A record for the states that enacted lottery-style programs to incentivize vaccine recipients. 

	Guaranteed Incentive -  A record for the states that guaranteed incentive rewards for vaccine participants. 

By analyzing these specific variables, our first project aims to uncover if there is a direct impact on vaccination incentives and policy measures about the amount of vaccines distributed. 

#### BUSINESS PROBLEM/HYPOTHESIS

The business problem we are addressing in this study is determining the effectiveness and, therefore, the need for vaccination incentives for vaccine rate influences and the subsequent public health outcomes. We hypothesize that vaccination incentives have a positive correlation with the overall vaccination rates and that the states that have implemented these public health programs will demonstrate higher dose administration than those without such programs. 


#### METHODS/ANALYSIS

Our data scientist's methodology was structured into four phases, focusing on analyzing the impact of incentive programs based on rates across each U.S. State. We have linked data from the CDC and different academic studies to examine the effectiveness of other public health strategies in enhancing vaccination rates. 
Phase 1: Data Collection and Wrangling 

The data wrangler for this project collected data from two primary sources. The first is the CDC's Global Covid–19 Vaccine Tracker, and the second is the JAMA Network on state–level vaccine incentives. The initial task was assessing the data quality and preparing it for analysis. This process involved: 

	Identifying and correcting any inconsistencies in data types.

	Handling missing values, especially in critical fields like vaccine distribution and administration rates.

	We are standardizing categorical data, such as incentive types, to ensure consistency across the datasets.


Phase 2: Exploratory Data Analysis (EDA)
After the data was cleaned, our team conducted an EDA to understand the distribution and correlation between the variables. Our primary steps included: 

	Utilizing map charts to visualize the distribution of states and their applicable dosage administration. 

	Employing heat maps for the Total Doses vs. State Incentive Lotteries. 

Phase 3: Comparative Analysis

Our comparative analysis was focused on the effectiveness of the different incentive strategies we listed between state-hosted lotteries and guaranteed incentives. 

	We compared vaccination rates between states with various incentive programs (e.g., lotteries, guaranteed incentives) against those without.

Phase 4: Statistical Modeling

To predict and interpret the impact of the vaccination programs, we applied statistical modeling techniques: 

	Regression models were used to assess the influences of public health policies and incentives on vaccination rates. 

	We refined our models, incorporating only the statistically significant variables to enhance the accuracy and relevance of our findings. 

#### RESULTS

Preliminary analysis indicates that there is, in fact, no significant association between a public health vaccination incentive and the overall number of administered doses. States with public health programs did not exhibit any significant difference in COVID-19 administered doses compared to those without one. 

We started by filtering the dataset for 'Yes' values in 'Lottery' and 'Guaranteed Incentive', calculating the z-scores for 'Doses distributed per 100k pop' for each 'State' for both 'Lottery' and 'Guaranteed Incentive', and then assess the association using a t-test between the z-scores of the two group
The t-test result indicates a statistic value of ~ 1.776e-15 and a p-value of ~ 0.9999999999999987.
Since the p-value is greater than the significance level of 0.05, we fail to reject the null hypothesis. This suggests that there is no significant difference in the means of 'Doses distributed per 100k pop' between the groups with 'Lottery' and 'Guaranteed Incentive' as 'Yes' compared to those as 'No.'
Therefore, based on this analysis, there doesn't seem to be a significant association between 'Lottery' and 'Guaranteed Incentive' and the distribution of doses per 100k population across states.

#### RECOMMENDATIONS/ETHICAL CONSIDERATIONS

 Based on our findings from the final analysis, we recommend policymakers prioritize fighting misinformation and pushing more public health programs aimed at informing the public of true information regarding the virus and the vaccines. We believe that creating more vaccinated individuals would be more beneficial than any public health program that monetarily rewards people for their vaccination status. Ethical considerations would include ensuring transparency in handling sensitive information regarding the vaccine and virus and trying to mitigate potential biases in vaccine manufacturers, effectiveness, and distribution. 

#### CONCLUSION

To conclude, our team study highlighted how there is no way to persuade the public to receive the vaccine monetarily. By leveraging statistical and comparative analysis, we have identified key insights into the effectiveness of public health interventions during the COVID-19 pandemic. We believe these findings have implications for potential future vaccination strategies and any pandemic preparedness efforts. 

#### REFERENCES

1.	CDC. (2020, March 28). COVID Data Tracker. Centers for Disease Control and Prevention. https://covid.cdc.gov/covid-data-tracker/
2.	COVID-19: Data on vaccines - NYC Health. (n.d.). https://www1.nyc.gov/site/doh/covid/covid-19-data-vaccines.page
3.	Coronavirus disease (COVID-19) – World Health Organization. (2024, April 5). https://www.who.int/emergencies/diseases/novel-coronavirus-2019
4.	Pfizer coronavirus resources: COvid-19 updates, news, information | Pfizer. (n.d.). https://www.pfizer.com/science/coronavirus/vaccine
5.	National Institutes of Health (NIH). (n.d.). National Institutes of Health (NIH). https://www.nih.gov/
6.	 Journal of Public Health Policy | palgrave. (n.d.). https://www.palgrave.com/gp/journal/41271
7.	U.S. Department of Health and Human Services. (2021). Vaccines National Strategic Plan 2021–2025. In Vaccines National Strategic Plan 2021–2025 [Report]. https://www.hhs.gov/sites/default/files/HHS-Vaccines-Report.pdf
8.	US Department of Health and Human Services/Centers for Disease Control and Prevention/National Center for Immunization and Respiratory Diseases. (n.d.). Increasing COVID-19 Vaccine Uptake among Members of Racial and Ethnic Minority Communities: A Guide for Developing, Implementing, and Monitoring Community-Driven Strategies. https://www.cdc.gov/vaccines/covid-19/downloads/guide-awardees-community-driven-strategies.pdf
9.	Hogan, C., Parzuchowski, A., Lyu, X., Goldstick, J. E., & Resnicow, K. (2022). Characterization of US state COVID-19 vaccine incentive programs. JAMA Network Open, 5(10), e2235328. https://doi.org/10.1001/jamanetworkopen.2022.35328
10.	Hacisuleyman, E., Hale, C., Saito, Y., Blachère, N. E., Bergh, M., Conlon, E. G., Schaefer-Babajew, D., DaSilva, J., Muecksch, F., Gaebler, C., Lifton, R. P., Nussenzweig, M. C., Hatziioannou, T., Bieniasz, P. D., & Darnell, R. B. (2021). Vaccine Breakthrough Infections with SARS-CoV-2 Variants. New England Journal of Medicine/the New England Journal of Medicine, 384(23), 2212–2218. https://doi.org/10.1056/nejmoa2105000
11.	J.R Zahar, D. Seytre, P. Moenne-Locoz, A. Lomont, & Y. Tandjaoui-Lambiotte. (2022). Spread of viruses, Which measures are the most apt to control COVID-19? National Library of Medicine. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9746078/
12.	12 COVID-19 vaccination strategies for your community. (2022, November 29). Centers for Disease Control and Prevention. https://www.cdc.gov/vaccines/covid-19/vaccinate-with-confidence/community.html






