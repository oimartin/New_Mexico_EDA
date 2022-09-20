# INTRODUCTION
**Goal:** Investigating economic data from New Mexico, USA in order to understand popular industries, demographic trends in industries, and change over time in employment. Data is organized by counties or by metropolitan statistical areas. Further comparisons are made between top performing county, Los Alamos, and low performing county Albuquerque MSA or Bernalillo County. 

As of 2021, NM total population was 2,115,877 and from 2016 - 2020, the average percentage of adults 16+ years of age participating in the labor force was 56.9% (link). The data covers time before the COVID-19 pandemic, before 2020, and some during the first few years of the COVID-19 pandemic from 2020 - 2021. I’m curious to see what the effect the pandemic had on employment and how healthcare related industries have fared in NM. 

# REQUIREMENTS
- Colab
- Python - pandas, matplotlib.pyplot, seaborn

# DATA
## Downloaded from - New Mexico Department of Workforce Solutions
https://www.jobs.state.nm.us/vosnet/Default.aspx?enc=vLa15KtdCzQQMP6jrcRdIQ==
### Current Employment Statistics
- From: Current Employment Survey
- Specific: Current workforce of NM (*not* farm work, supervisory roles, armed forces, self-employed, proprietors, domestic workers, unpaid family workers, railroad workers, look for work)
- Years: 2017 - 2021

### Local Area Unemployment Statistics
From: Current Population Survey
Org: Federal-State cooperative
Years: 2017 - 2021

### Quarterly Census of Employment and Wages
Org: Bureau of Labor Statistics and the State Employment Security Agencies
Years: 2017 - 2020

### Occupation Employment Projects
From Occupational Employment and Wage Statistics Report 
Org: Bureau of Labor Statistics
Years: 2018 - 2028

### Comparative Economic Characteristics
From American Community Survey
Org:  US Census Bureau
Years: 2013 - 2017

The following data, Current Employment Statistics, Local Area Unemployment Statistics, Quarterly Census of Employment and Wages, and the Occupational Employment Projections, have suppressed data categories. Government/public sources are required to suppress data for small populations when releasing the data to the public. The Comparative Economic Characteristics data was aggregated over the years 2013-2017, so no data is suppressed since the data is just an estimate for the time frame. The data was downloaded in July 2021.

# INSIGHTS
## Current Employment Over the Years
The figure shows the positive progression most industries were experiencing with an increase in the number of employees from 2017-2019. 2020 saw the most dramatic decline of employees, and 2021 continued to see a decline in the number of employees.
[New_Mexico_No_Employee_Change_By_Industry_17_20.png]

## County Unemployment Over the Years
The unemployment data includes MSA, or metropolitan statistical area, and counties. We see that Bernalilo County and Albuquerque MSA fall in the lower half of the unemployment rate. This was the first place to see that Los Alamos county seems to consistantly have a low unemployment around 3%. Also, Luna County is consitantly has the highest unemployment rate through the years. Similar to the employment data, most counties/MSA's were experiencing a decline in the unemployment rate from 2017 - 2019, and in 2020, experienced an increase in the unemployment rate. Depending on the county, the unemployment rate increased or decreased in 2021. In 2021, the unemployment rate in Luna county increased, and in Los Alamos county, it decreased.
[Unemployment Rate by County 2017-2020.png]

## Los Alamos, Bernalillo, and Luna County Comparisons by Top and Low Earning Industries
In Los Alamos county, the Real Estate industry either combined or separately private has the highest median average weekly wage. The other top industries in Los Alamos median average weekly wage slightly above 1000 when just private employers and under 1000 for private and public employers. The Healthcare and Social assistance industry has a median average weekly pay of about $600 with public or private employers.
[ALL_Los_Alamos_County_AvgWklyWrkr_Industry_Title_combine_2017-2020.png,  Priv_Los_Alamos_County_AvgWklyWrkr_Industry_Title_combine_2017-2020.png]
In Bernalillo county, The highest median average weekly pay for Bernalillo county, among public and private employer, was Funds, Trusts & Other Financial Vehicles, and National Security & International Affair.The lowest performing industries were Clothing and Clothing Accessories Stores and Sporting Goods/Hobby/Book/Music Stores. For private employers, the Pipeline Transportation industry and Funds, Trusts & Other Financial Vehicles industries were the top median average weekly pay. The Healthcare and Social Assistance industry has a median average weekly salary of under 1000, for public or private employers.
[ALL_Bernalillo_County_AvgWklyWrkr_Industry_Title_combine_2017-2020.png, Priv_Bernalillo_County_AvgWklyWrkr_Industry_Title_combine_2017-2020.png]
Similar to Bernanillo county, the highest median average salary is in the Financial Investment & Related Activity industries among public and private employers in Luna County. Membership Organizations & Associations and Wood Product Manufacturing are also high paying industries for public and private employers. The lower paying industries include Accommodation and Performing Arts & Spectator Sports for both public and private employers. For just private employers, the top paying industries are: Printing and Related Activities and Heavy and Civil Engineering and low paying industries are: Accomodation and Personal & Laundry Services. Healthcare & Accommodation among public and private or exclusively private employers is below $1000 average weekly pay.
[ALL_Luna_County_AvgWklyWrkr_Industry_Title_combine_2017-2020.png, Priv_Luna_County_AvgWklyWrkr_Industry_Title_combine_2017-2020.png]

## Occupations Expected to be Most Needed
Information security analysts are expected to grow at a rate between 3.6 and 3.7 in Albuquerque MSA and New Mexico. This data was taken in 2018 prior to the COVID-19 pandemic, so it will be interesting to see how the growth rate actually performs. After generating the first table for New Mexico, I see that personal care aides, an occupation related to health care, is expected to grow by 3.2 percent annually. On the lower growth rates, Postal Services occupations are expected to decline between 2.7 and 3.2 percent, Albuquerque and New Mexico, respectively.

[graph?]

## Economic Characteristics by County
One of the strongest correlations of economic characteristics is between the total amount of a household's median income and the population of people 16 years and older who are not in the labor force, at -0.69. This association between income and labor force makes sense as less people in the workforce would have a lower income. The other strong correlation is between non-family households median incomes with females working full time and the total households median incomes, at 0.88 . In terms of working population, Bernalillo county has the highest number of workers by almost 3 times that of Doña Ana County, the second highest number of workers.
[working_population_by_county.png, proportions_of_population_by_counties_economic_characteristics.png,
Correlation_matrix_economic_characteristics.png,
Household_income_all_and_femaleFT_all_counties.png]
