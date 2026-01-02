# The Effect of Rising Social Media Usage on Shopping Behaviour

## Project Overview
In this project I will focus on the correlation between the widespreading usage of social media and the usage effects of the things people buy. Main aim is to find if social media influences people to buy and consume more. By analyzing datas on how much time people spend online and how often they shop online, it is expected to find a correlation between these parameters within this project outcomes. 

The analysis will rely on statistical methods and visualization techniques combining screen time data, demographic information and Google Trends search interest.By examining this relationship from different aspects, this project aims to determine whether social media exposure is a meaningful predictor of consumer interests accross countries alone. 

## Motivation
Social media has evolved into one of the most influential environments in modern life. It creates trends and products then turns them into cycles of consumption. I believe that the constant exposure to these trends evolves into a strong link between online engagement and consumer behavior as far as I inspected in day to day life. My main motivation is to discuss if constant exposure to social media really alters consumption habits.

My motivation is to move beyond the intuition and use real data to test whether increased social platform exposure turns into measurable changes in consumer interests. Understanding this relationship is valuable for:

- Evaluating the real impact of digital exposure on consumption patterns
- Distinguishing real correlation rather than keeping it only as an assumption 
- Understanding whether dempgraphic or platform based factors improves the predicitons

## Research Question and Hypothesis

**Research Question:**

Does increased social media usage lead to higher consumer interest in online shopping?

**Null Hypothesis:** 

There is not a significant relationship between daily social media usage and consumer behaviour in online shopping.

**Alternative Hypothesis:** 

Increasing social media usage indicates an increase in consumer interest in online shopping and consumerism.

## Data Sources and Collection
For this project I am going to make use of the dataset I found on Kaggle. For the second dataset, I am going to use Google Trends datas with pytrends. To process these datas, I am going to use Python libraries such as numpy, pandas and matplotlib. First dataset will include screen time information with mostly used social medias and countries. From Google trends I will facilitate the data on shopping sites. This data integration will result in constructing a coherent analytical framework and better visual representation. Cleaning, standardization, and normalization steps will ensure comparability across the datasets. 
In this project I make use of three main datasets:

**1. Screen Time and Demographics**
- Dataset from Kaggle
- This dataset includes:
    - Average daily social media usage (hours)
    - Country
    - Age and gender information
    - Most frequently used social media platform

**2. Google Trends Search Interest Data**
- Dataset collected using pytrends from Google Trends
- Used as an indicator for consumer interest
- This dataset includes:
    - Country-level search interest for a popular online shopping keyword (Popmart)

**3. Engineered Country-Level Features**
- Engineered from the online datasets I collected
- All datas cleaned and aligned by countries 
- This dataset includes:
    - Demographic statistics 
    - Platform usage details
    - Average usage observations per country

## Explanatory Information for the Project
The first dataset found from Kaggle is the important dataset for the screen time datas. Besides the screen time column, I am also going to make use of other columns suchs as country and most frequently used social media platforms. This dataset is from 2025. I am going to relate these datasets to shopping behaviour. After a research on how to achieve this, I decided to search for the 2025 trends of social media and the trends on purchased items. The dominating purchase for the 2025 trends was including categories such as Labubus (some kind of a monster toy). After the research, I found out that these products are originally sold in online shops called Pop Mart. So I decided to see the interest rates of countries on Google searching the keyword "Pop Mart". In the next steps of my project, I am going to see if the average screen times of these listed countries have any sort of relation between the interest in these shopping places.

## Exploratory Data Analysis (EDA) Steps
First I get the dataset I found from Kaggle in csv format. Then I choose between the columns the ones I need for my analysis. I apply cleaning steps for this data to handle any missing values or unrelated outcomes. Lastly I keep the cleaned data in another csv to use it for my further analysis. Next step, I install pytrends to reach the data I need from Google Trends. In this step I get the searched word's interest rate for each country in my cleaned csv. I do the cleaning by deleting the countries that have no data on that word. Later, I found the interquiartile ranges and detected any outliers. 

The EDA phase mainly focused on:
- Removing invalid values (e.g., screen time > 24 hours)
- Handling missing datas
- Detecting and removing outliers using interquartile range (IQR)
- Visualizing distributions and relationships between variables

During this step, the initial scatter plots and correlation checks showed a weak linear relationship between screen time and consumer interests.

## Methodology

**1.Hypothesis Testing**

I used correlation analysis to test the relationship between:
- Average daily social media usage
- Average Google search interest

Results did not provide strong statistical evidence to reject the null hypothesis. So the results indicate that there is not a significant relationship between daily social media usage and consumer behaviour in online shopping.

**2.Regression Models**

I used and tested the regression models below to predict average search interest:
- Linear Regression
- Polynomial Regression
- Decision Tree Regression
- KNN Regression

I used Root Mean Squared Error (RMSE) and R² score to evaluate the tested models. Across all regression models, R² was consistenly negative showing that none of these models performed better than predicting the mean search interest.

**3.Feature Engineering**

After evaluating the regression models I tried additional features to improve model performance. The features I added:
- Mean age per country
- Gender distribution
- Platform usage proportions
- Number of observations per country

Despite the features I added, the regression still performed weakly indicating that the relationship is either nonlinear, other unobserved factors are present or fundamentally weak.

## Key Findings
- Average daily social media usage is not a strong predictor of consumer interests alone
- Adding new features linked with demopgraphical and platform-related aspects improved the interpration but did not changed the overall predictability 
- All regression models failed to outperform a mean based baseline

## Conclusion and Limitations
I aimed to demonstrate that while the social media usage is often associated  with driven consumer behaviours, in fact, screen time is not a sufficient parameter to correctly predict consumer interest alone. Consumer behaviour appears to be affected by a more complex combination of factors that are not fully available and captured in my datasets. Still the findings on weak relation is important to furtherly challenge this common assumption and highlighting the limitations.






















