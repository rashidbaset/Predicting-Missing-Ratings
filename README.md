- [Objective in business terms](#business-objective)
- [How is the business problem handled today?](#business-objective)
- [How will the solution be used?](#how-will-the-solution-be-used)
- [Consequences of predicting wrong solution, cost of false positive?](#how-will-the-solution-be-used)
- [How will model be deployed?](#how-will-the-solution-be-used)
- [Who is going to use the model?](#how-will-the-solution-be-used)
- [How will the output of the model be represented?](#how-will-the-solution-be-used)
- [Current solutions/workounds (if any)?](#current-solutions-workarounds)
- [Framing the problem](#framing-the-problem)
- [How should performance be measured?](#how-should-performance-be-measured)
- [Is the performance measure aliged with the business objective?](#data)
- [Minimum performance needed to reach business objective?](#eda)
- [Comparable problems? Can you reuse experience or tools?](#modeling)
- [Methodology](#evaluation-metrics)
- [List of assumptions made so far](#modeling)
- [Verify Assumptions if possible](#modeling)
- [Next Step Future Work](#nextstep-futurwork)
- [References](#references)

## Business Objective

How can we identify a brand's reviewers who are most likely to respond to marketing campaigns for digital movie purchases? Using prior reviewer ratings data and a recommendation engine to predict the probability of missing ratings from reviewers and suggest users with 80% or greater favorability. 

## How will the solution be used?

A. Content Based Recommender Engine
B. Item and Attribute selling 

## Current Solutions/workarounds? 

## Framing the problem

- In this fictional scenario, Blockbuster.com is in it's last stages before bankruptsy and are considering creating a recommender system based on ratings data from their 600 online movie reviewers. They are contracting out bids and are considering our firm and apropriating our recommender model. 

- New user registration the movie ranking site, MovieRatings.com, has 

## Ignore all movie-ranking sites 

- What is the business objective? 

Improving 

### Understanding the data


## Data files with features 
|                            	| Features                                     	|
|----------------------------	|----------------------------------------------	|
| ```df_movie_ratings.csv``` 	| movieId, title, genres, userId, rating 	|
| ```movies.csv```           	| movieId, title, genres                 	|
| ```ratings.csv```          	| userId, movieId, rating, timestamp   	|
| ```tags.csv```             	| userId, movieId, tag, timestamp     	|

## Features and their description 
|                 	| Features         	|
|-----------------	|------------------	|
| ```userId```    	|  610 unique user ids, 0.6% unique              	|
| ```movieId```   	|  9,724 distinct count, 9.6% unique              	|
| ```title```     	|  9,719 distinct count, 9.6% unique                	|
| ```genres```    	|  951 distinct count, 0.9% unique                	|
| ```rating```    	|  Movie rating score. 0.5 - 1.0, 5.0 most favorable, 3.5 is the mean.                	|
| ```timestamp``` 	| Unable to determine 9 digit timestamp. ('1537110021')                 	|
| ```tag```       	|  Keywords selected by the reviewer.                	|


## How should performance be measured?

## Is the performance measure aliged with the business objective?

## Methodology

We want to first try and determine most active reviewers or reviewers who are most likely to show movie purchase propensity when viewing advertisements for the movie.

Next, what are different combinations of genres and tags that have the most reviewers. 

Clustering models/users--assign user to the segment containing the most similar reviewrs. 

Determine favorite movies based on ML on missing data. 

Compare results from clustering modeling and missing ratings prediction. 

## Suggestion

--

A. How will file be used?
B. Recommend similar movies to users based on ratings 
  high value reviewers, or to find reviewers  who are similar to active the reviewer , cluster models divide the customer base into many segments and treat the task as a classification problem. The algorithm’s goal is to assign the user to the segment containing the most similar customers. It then uses the purchases and ratings of the customers in the segment to generate recommendations.

## References 
[1] https://towardsdatascience.com/for-your-next-project-i-recommend-ab89cad53dec
[2] https://www.wired.co.uk/article/which-film-ranking-site-should-i-trust-rotten-tomatoes-imdb-metacritic

