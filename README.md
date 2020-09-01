# Analysis of the UN's World Happiness Index with machine learning

Maaike de Jong  
June 2020

## Introduction
The World Happiness Report is an annual publication of the United Nations Sustainable Development Solutions Network. It presents the results of a survey of the state of global happiness that ranks 156 countries by how happy their citizens perceive themselves to be. The rankings of national happiness are based on a Cantril ladder survey, where nationally representative samples of respondents are asked to think of a ladder, with the best possible life for them being a 10, and the worst possible life being a 0. They are then asked to rate their own current lives on that 0 to 10 scale. 

There are large differences in happiness among countries and continents, with usually the top happiest countries from Western Europe, and the least happy countries from sub-Saharan Africa and the Middle East. In this analysis I use machine learning to investigate which factors are important in determining the overall happiness score of nations. Specifically, I aim to answer the following questions:  
  
**1. Which economical, social and environmental factors contribute most to a country’s happiness?**  
**2. How well can we predict happiness score with these factors?**


## Analysis
I use scikit-learn's linear regression model with recursive feature elimination to analyse the contribution of 20 World Development Indicators (WDIs) with the World Hapiness Score. I used the average Happiness score of the past five years, and started with the following WDIs per country for the past 10 years:
* Access to electricity (% of population)  
* CO2 emissions (metric tons per capita)  
* Compulsory education, duration (years)  
* GDP growth (annual %)  
* GDP per capita (current US$)  
* Individuals using the Internet (% of population)  
* Land area (sq. km)  
* Life expectancy at birth, total (years)  
* PM2.5 air pollution, mean annual exposure (micrograms per cubic meter)  
* People using at least basic drinking water services (% of population)  
* Population density (people per sq. km of land area)  
* Population growth (annual %)  
* Proportion of seats held by women in national parliaments (%)  
* Refugee population by country or territory of origin  
* Population, total  
* Renewable energy consumption (% of total final energy consumption)  
* School enrollment, primary (gross), gender parity index (GPI)  
* Terrestrial protected areas (% of total land area)  
* Urban population (% of total population)  

## Data
The World Happiness Report data from 2015-2019 can be found on [Kaggle](https://www.kaggle.com/unsdsn/world-happiness) (five separate csv files).  
I retrieved a csv file with 1400+ World Development Indicators for all countries from the [World Bank's website](http://datatopics.worldbank.org/world-development-indicators/) (under 'Bulk Downloads').

## File structure
The analysis is divided over four notebooks:
1. Data wrangling to combine the different datasets
2. Data cleaning and visual exploration
3. Regression analysis with scikit-learn
4. Visualising the data in graphs and world maps


