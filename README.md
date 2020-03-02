# Road Safety-Safety Always Matter!!

This project is to analyze the relationship between accident occurrence rates and factors that contribute to them. What is meant by accident occurrence rates is how often road traffic deaths are prone to happen in a country. This project helps in understanding which factors affect accidents in countries. One factor that could potentially affect the occurrence rate of accidents in a country is not following best practices. The data will describe which factors are related to road traffic deaths in each country and how the existence of national policy on public transport affects the rates. This information is vital for countries to avoid the number of casualties that occur yearly. The better informed a nation is of what factors affect accidents, the more equipped they can be to address those factors. They can correct those factors with more law enforcement and other measurable, actionable steps that include strategies to reduce the occurrence rate of accidents.

**Data Source:**

http://apps.who.int/gho/data/node.main.A989?lang=en

**Dataset Description:**

The dataset is compiled with information collected from over 140 countries between the years of 2013 and 2016. The data we collected is from the World Health Organization (WHO) website, which is a credible organization that has more than 7000 people working in 150 country offices. A subset of the data includes information regarding the estimated number of road traffic deaths and an estimated number of road traffic deaths per 100,000 population. In the data, there is information on the distribution of road traffic deaths by the type of road users. Lastly, the data also has information about training in emergency medicine.

**Data Engineering:**

1.	Merging data from different comma separated values (csv) files according to the countries and managing missing data.

2.	Some of the data pertaining to different countries is missing. For example, the number of registered deaths from two wheelers in a    particular country is not available or there are countries for which clear information regarding the availability of emergency training program, regulations regarding road safety are missing. For the missing data, we use some functions like ‘pandas.DataFrame.fillna’ to fill it.

3.	Some value contains unwanted characters like ‘~’, ‘-‘, we use some functions like Series.str.extract() to cope with it.

4.	Some column names are missing, so we use some methods like ‘pandas.DataFrame.rename’ to fill the empty columns. 

5.	Converting data type In dataframe, the type of data is not numeric, we use pandas.to_numeric or numpy.ndarray.astype to convert the data type to numeric for future analysis. 

6.	Merging different dataFrames For better analysis, sometimes data from two or more files is needed, so pandas.DataFrame.merge used to merge two dataframes.

**Conclusion:**

*	High income countries own more than 20 percent of the cars in the world whereas low income countries own just 2 percent of the cars, but low-income countries have more than 20 percent of the road deaths compared to high income countries. With this we could conclude that Low income countries must improve their rules and regulations tremendously to reduce the road deaths.

*	The road traffic deaths rates involving alcohol for countries following BAC Law with best practice are low and no more than 20%, while in countries without best practice the road traffic deaths rates are higher. Therefore, it's better for countries to follow BAC Law with best practice.

*	For countries following best practices, 30% countries have 10-15 % road traffic deaths involving alcohol whereas for countries that violates atleast one best practices 30% countries have 0-5 % road traffic deaths involving alcohol. For countries following BAC laws, almost 65% countries fall below the (10-15)% category, same is the case with countries following BAC laws with best practices. Although, some countries has moved towards (0-5)% bin but also there are countries which has moved towards (75-80)% bin. Therefore, following best practices doesn't have a great impact on reducing the % road traffic deaths involving alcohol.

*	Also found out Bhutan has the highest number of deaths when compared with its population.

*	Another key finding was countries which promote lot of walking and cycling culture have relatively less road deaths compared to countries which do not promote this culture. We could also help different countries by showing them the analysis and tell them importance of cycling and walking culture.

*	Lastly with this project we could also understand about the countries policies, how strict laws are in different countries and where different countries lack in the safety measures.
