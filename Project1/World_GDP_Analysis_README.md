# World's GDP Exploration
## by Hassanat Awodipe


## Dataset

The dataset was gotten from [kaggle](https://www.kaggle.com/datasets/truecue/worldsustainabilitydataset?select=WorldSustainabilityDataset.csv) and it was compiled from World bank. It contained two tables: **World Sustainability dataset** which contained the economic data of countries in the world from 2000 t0 2018 and the **Data dictionary** which described the features in the table.

The table contained a number of nulls rows. For the important columns: GDP and Population, I dropped the null rows. For this reason, my analysis started from the year 2001 with 3,072 observations from 172 unique countries. This data cleaning process was done in MS Excel. The supporting numeric columns such as `exports`, `imports` had few missing rows which made up 13% of the data. I examined these columns individually to understand the pattern; some regions consistently had missing data for all the years.


## Summary of Findings

During the exploration, I found out that there was a strong positive correlation between GDP and Population but the increment in GDP was influenced by other factors such as exports, imports, inflation, total natural resources, gross savings and gross national expenditure. There was a drop in GDP in 2015 and this year experienced a high amount of negative inflation. This supported an earlier bivariate analysis that showed that there was a strong negative correlation between GDP and inflation.

When considered as a whole, GDP(2001-2018) shows a negative correlation with exports. This supported the paradox of plenty theory. However, when the GDP(2010-2018) and Population was examined with exports, the relationship resemebled the export-led growth theory. This showed that effect of exports on different countries GDP is not the same.

Sub-Sahara Africa region had the highest count of observations while High Income Class occurred the most in the dataset. Even with these, more points of Sub Sahara Africa consistently showed up in Low income when Regions and Income Class were plotted against the numeric features. Eastern and Southern Asia had points scattered around all Income Classes. Europe and Northern America & Northern Africa and Western Asia always had noticeable points in the High Income and Upper middle income Class.   

The average GDP Per Capita was outrageously high for high income class compared to the other income classes for all 7 regions. Central and Southern Asia had no count for high income class  

## Key Insights for Presentation

For the presentation, I will mainly focus on **GDP, population and income class**. I would show how the growth of population corresponds to that of GDP and then the effect of inflation on GDP while population increased. I will start by introducing the distribution of
GDP then compare GDP to population over the years that the data was collected. I will then introduce the inflation variable which has the strongest negative correlation with GDP and show how it can contribute to the fall of the GDP even when population increases. GDP fell in 2015 and there were a lot of deflation in 2015 and 2016. 

Thereafter, I will introduce the categorical variables and show their distribution with GDP. I will then use the **GDP per capita** feature to illustrate the effect of Population on GDP by regions and income class. 
