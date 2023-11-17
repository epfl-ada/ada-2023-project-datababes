# Brew to success 🍻

## Abstract
Brewing the perfect beer is a task many set out for and only a few, if any, even achieve. When it comes to crafting a beer, choosing the right ingredients, temperature, brewing equipment and overall recipe design is crucial while leading to an explosion of possibilities. It is this vastness of possibilities that captivates so many brewers around the globe chasing the perfect beer.<br>
With our project we aim to break the flood of information supplied by the beer rating websites [BeerAdvocate](https://www.beeradvocate.com/) and [RateBeer](https://www.ratebeer.com/) down into easily digestible pieces of information, leading to meaningful insight for interested readers and might even increase their chances of brewing a well liked beer.<br>
Do you prefer to stick to the same three popular types of beer that you know, or would you be ready to immerge yourself into the world of beers and discover a choice that perfectly matches the mood of the month ?


## Research Questions
What would be the ideal beer for the US consumer depending on the month?

To answer this question we are going to look at different aspects:

📌 How does the location of the different breweries affect the ratings?

🌀🌿💘🔥 & 📖 Rate reviews and keywords appearing in them by combining sentiment and dictionary analysis. What keywords are carry the most positive sentiment? What keywords are used in a negative way? This analysis can give an indication of what emotions a beer should evoke.

🍷‰ Does the alcohol content lead to a perceiveable change in ratings or review sentiment?


Assumptions:
- The popularity of beer is correlated to the numbers of good ratings received. A good rating is defined to be of higher value than the average rating of the entire dataset.
- Beer reviews and ratings are written close to the time of consumption (on the same day).


## Methods

### Time series analysis
The time series analysis is the direct consequence of our aim to analyse how the perfect beer evolves over the months of the year. For this the review data is layered on top of each other with the period being one year and twelve bins, representing the twelve months, are established.
We will use this to analyse and present different attributes such as keyword frequencies and the value of ratings.

### Dictionary analysis
The dictionary analysis allows us to see what words are used in each month to describe a beer. Paired with the sentiment analysis we can then conclude from this what aspects of the beer are more valued depending on the month.

### Sentiment analysis
By using sentiment analysis we can map reviews and potentially also words from the dictionaries we use to a positive-negative sentiment scale, which allows us to verify and better understand the reviews themselves.

### T-tests
We will use t-tests to give our assumption some statistically expressed support by quantifying significances. More specifically, for beer styles that are present in the top 20 only in certain months, we will check if that difference in good ratings is stastitically significant.


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

## TA Questions
- library definition: Currently we did a manual research to create our library. We might get more adapted results by first running an analysis of the reviews to create the word library, and then using it to analyse the dataset. But we are not sure if this might lead in a wrong direction.
- Popularity is related to the number of unique users that rate the beer. We want to limit the effect of a small but very communicative fan group from having too much of an impact on the rating of a beer and develop a threshold limit per user and beer. What do you think about this consideration and how should we integrate this ?

<!--
## Project Proposal (Milestone 2)

Whatever set of combinations of these two aspects is chosen can then yield recommendations on how to produce and launch a successful beer. Successfulness is measured by ratings and only the top X beers for a certain Group and Time are chosen.
Examples:
- For the group of type `Lambic` in `January` we only look at the beers `a`, `b` and `c` as they are considered the most successful with their average rating of 4.6, 4.58 and 4.52 accross all recorded januaries.
- For the group of type `Imperial IPA` in `2011` we only look at the beers `x`, `y` and `z` as they are considered the most successful with their average rating of 4.6, 4.58 and 4.52 across 2011.

We decided not to proceed with the `matched_beer` dataset initially supplied as merging the datasets of `BeerAdvocate` and `RateBeer` provides a more complete dataset.
-->
