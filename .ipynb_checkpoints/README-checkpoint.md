# Training project in Data Science

If you would execute this notebook in your host, run this comand in folder terminal:

** jupyter notebook**
or
** jupyter lab**

## Problem situation


You are contracted to help a movies producer company to explore information about movies genre. The Idea is to get a information about ratings, popularity, production date and movie genre.

In your first work with data scientist is do a EDA(exploratory data analysis) with this database.

## Utilized libraries
* Pandas
* Seaborn
* Scipy
* Matplotlib

## Normality test
 
* Anderson: evaluate what kind of distribuition about data, return many values in addition to the p value.
* Shapiro-Wilk: evaluate if samples have gaussian behavior, is useful for a small datasets
* D'Agostino ou K² test: return a statistic summary about data.

## Some point in this project

* There are films with more than one category, this can lead to a vote counting a little more than others, in addition, some categories may have number of votes
very close, as is the case with drama and action films, that is, if you are voting for a film you may be voting in two or more categories.

* If dividing the number of votes by the number of films results in war films having the highest value, this brings many conclusions, as
that there are few films and a lot of votes in them, so this can show users interest in these types of films. With that, the film war category is easier to
fit in with other categories, that is, it is easier to see a film labeled as war/romance or war/drama than documentary/romance.

* There was something from the 1990s that the production of films in all genres increased, with that, it was necessary to analyze the correlation between the columns or parameters
dividing the feeders before and after this season.

* Based on total votes, the most watched movies from the 1990s are drama movies followed by a small difference a
action category. Comedy films were in the lead before the 1990s (but, of course, there are many more films after that time) followed by a small differences in action movies.
