# Brew to success 🍻

## Abstract
Brewing the perfect beer is a task many set out for and only a few, if any, even achieve. When it comes to crafting a beer, choosing the right ingredients, temperature, brewing equipment and overall recipe design is crucial while leading to an explosion of possibilities. It is this vastness of possibilities that captivates so many brewers around the globe chasing the perfect beer.<br>
With our project we aim to break the flood of information supplied by the beer rating websites [BeerAdvocate](https://www.beeradvocate.com/) and [RateBeer](https://www.ratebeer.com/) down into easily digestible pieces of information, leading to meaningful insight for interested readers and might even increase their chances of brewing a well liked beer.<br>
Do you prefer to stick to the same three popular types of beer that you know, or would you be ready to immerge yourself into the world of beers and discover a choice that perfectly matches the mood of the month ?


## Research Questions
What would be the ideal beer for the US consumer depending on the month?

To answer this question we are going to look at different aspects from the eda.ipynb notebook.

📌 How does the location of the different breweries affect the ratings?

🌀🌿💘🔥 & 📖 We want to know the best characteristics defining each category (such as taste or color), and to do so we extract popular keywords that are present in the reviews.

🍷‰ Does the alcohol content lead to a perceiveable change in ratings or review sentiment?


Assumptions:
- The popularity of beer is correlated to the numbers of good ratings received. A good rating is defined to be of higher value than the average rating of the entire dataset.
- Beer reviews and ratings are written close to the time of consumption (on the same day).


## Methods

### Pre-processing and Dataset Construction

In our pre-processing phase, we encountered the challenge of aligning two different datasets. One of the issue we had was the absence of consistent beer IDs across the datasets for identical beers, while similar IDs could be associated with different beers. To address this, we opted to generate new, consistent beer IDs for each entry.  
Additionally, the beer style names in the two datasets varied, which required a standardization. To tackle this problem we decided to map names from one dataset to the other, and to sometimes strategically map more specific styles from one dataset to broader styles in the other.  
To avoid getting mixed results that might be affected by the different tastes and seasons in different parts of the world, we decided to to filter our dataset to only keep ratings from people from the US as it is the region where users rated the most.  
Finally, and as a precautionary measure, we've decided to remove users with suspect behavior (such as the excessive rating of a beer in a short period of time) from the dataset to keep the reliability of the ratings.

### Time Series Analysis
The time series analysis is the direct consequence of our aim to analyse how the perfect beer evolves over the months of the year. For this the review data is layered on top of each other with the period being one year and twelve bins, representing the twelve months, are established.
We used this to analyse the changes of different beer characteristics across the year, and present different attributes such as keyword frequencies and the value of ratings.

### Keyword Analysis
We performed keyword analysis to find out what aspects of the beer are more valued depending on the month. To do this, we first used dictionary analysis uncover what words are used in each month to describe a beer. We then used clustering to group keywords that describe the same beer characteristics once we have extracted those keywords from the user reviews.  

### T-Tests and Mann-Whithney U Test
We will use these tests to give our assumptions some statistically expressed support by quantifying significances. More specifically, we used the Mann-Whithney U Test to show that the distributions of the ratings between US users and the others are significantly different which supported our decision to only focus on US users. We also used t-test to have statistical backing to our assumptions, like on the ratings of the two datasets to show that the ratings in the two datasets are significantly different.

### Observational Study
...TODO...

## Timeline
```
.
├── 20.11.23 - Pause project (HW 2)
│
├── 27.11.23 - Criteria analysis
│
├── 01.12.23 - Homework 2 deadline
│
├── 04.12.23 - Continued analysis of criteria
│
├── 11.12.23 - Finalize code, start with data story
│
├── 18.12.23 - Finalize data story
│
├── 22.12.23 - Milestone P3 deadline
.

```

## Team Organisation
- Cyril: Exploratory Data Analysis, Rating Keyword Analysis, Datastory
- Ajkuna: Exploratory Data Analysis, Rating Keyword Analysis, Website Creation, Datastory
- Alex: Project Proposal, Beer Location Analysis, Datastory
- Tim: Project Proposal, Alcohol by Volume Analysis, Datastory
- Dana: Exploratory Data Analysis, Pre-Processing for Dataset Construction, Datastory
