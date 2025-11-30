# The Effect of Rising Social Media Usage on Shopping Behaviour

## Project Overview
In this project I will focus on the correlation between the widespreading usage of social media and does this usage effects the things people buy. Main aim is to find if social media influences people to buy and consume more. By analyzing datas on how much time people spend online and how often they shop online, it is expected to find a correlation between these parameters within this project outcomes. 

The analysis will rely on statistical methods and visualization techniques to examine correlation strength, variation across countries and possible other parameters. The project will finally decide whether social media acts as a meaningful predictor of consumption habits or whether the relationship is weaker than assumed.

## Hypothesis
Null Hypothesis: There is not a significant relation between screen time and consuming behaviours.

Alternative Hypothesis : Increasing screen time will indicate an increase in consumerism meaning that there is a strong positive correlation.

## Motivation
Social media has evolved into one of the most influential environments in modern life. It creates trend and turns them into cycles of consumption. I believe that the constant exposure to these trends evolves into a strong link between online engagement and consumer behavior as far as I inspected in day to day life. My main motivation is to understand if constant exposure to social media alters consumption habits and which groups are affected by this exposure the most.

## Data Sources and Collection
For this project I am going to make use of the dataset I found on Kaggle. For the second dataset, I am going to use Google Trends datas with pytrends. To process these datas, I am going to use Python libraries such as numpy, pandas and matplotlib. First dataset will include screen time information with mostly used social medias and countries. From Google trends I will facilitate the data on shopping sites. This data integration will result in constructing a coherent analytical framework and better visual representation. Cleaning, standardization, and normalization steps will ensure comparability across the datasets. 

## Explanatory Information for the Project
The first dataset found from Kaggle is the important dataset for the screen time datas. Besides the screen time column, I am also going to make use of other columns suchs as country and most frequently used social media platforms. This dataset is from 2025. I am going to relate these datasets to shopping behaviour. After a research on how to achieve this, I decided to search for the 2025 trends of social media but the trends on purchased items. The dominating purchase for the 2025 trends was including categories such as labubus (some kind of a monster toy). After the research, I found out that these products are originally sold in online shops called Pop Mart. So I decided to see the interest rates of countries on the Google searching keyword "Pop Mart". In the next steps of my project, I am going to see if the average screen times of these listed countries have any sort of relation between the interest in these shopping places.

## EDA Steps
First I get the dataset I found from Kaggle as in csv format. Then I choose between the columns the ones I need for my analysis. I apply cleaning steps for this data to handle any missing values or unrelated outcomes. Lastly I keep the cleaned data in another csv to use it for my further analysis. Next step, I install pytrends to reach the data I need from Google Trends. In this step I get the searched word's interest rate for each country in my cleaned csv. I do the cleaning by deleting the countries that have no data on that word. Later, I found the interquiartile ranges and detected any outliers. Also deleted the outliers so it wwill not be leading my analysis.




















