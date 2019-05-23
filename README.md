# Udacity_IMDB_Movie_Dataset
A Udacity project of investigating movie dataset with Jupyter Notebook. In this dataset, there are provided information about movie details and informations from movies that are released during 1960-2015. The dataset contained movie details such as title, runtime, cast, genres, etc. and movie rating from imdb in popularity. We will conduct a research about the most popular genre year-to-year from 1960-2015 and the most influential traits (Popularity, Budget and Average Votes) that are associated with the high-revenue movies in this data.


# EDA Highlights 
## Research Question 1: Which Genre is the overall most popular year-to-year? 
After fixing the format problem (multiple genres entry changed into individual genre entry) for the movie genre, I found out that drama is the most popular genre overall from 1960-2015 by counting on their popularity with action genre following as the second most popular overall genre 

![The Most Popular Genre from 1960-2015](https://github.com/audichandra/Udacity_IMDB_Movie_Dataset/blob/master/Genre%20popularity%20bar%20chart.png)


## Research Question 2: What kinds of properties are associated with movies that have high revenues?
I wanted to investigate the following properties which can affect the movies revenue. The following variables (popularity, budget and vote) seems to have high impact toward the movies revenue which is why I conducted the following OLS regression of movies popularity, adjusted budget and vote as independent variables toward movies adjusted revenue as dependent variables. 

![OLS Regression Result](https://github.com/audichandra/Udacity_IMDB_Movie_Dataset/blob/master/OLS%20Regression%20Result.png)

The following OLS regression results obtained after several problems such as multicollinearity and normality fixed by Standardizations and Boxcox transformation. With this OLS regression results, we can find out that all of the independent variables (Popularity, Adjusted Budget and Average Vote) are significant and the adjusted R square explained that 56% of the dependent variables are explained by these independent variables. The most significant independent variables is Adjusted Budget. 

This result also inline with the line of reasoning that with more budgets, there will be more capabilities in producing good movies, thus, making more people to be interested to watch it and generating more revenues. Popularity or hype are also capable in influencing more people to watch the movie as well as vote or ratings that are becoming benchmarks for more people to watch again.

## Limitations 
For question no.1, the limitations located in the question itself which might be too broad, thus, making it harder to generate more information that can give useful informations. In terms of the research, it can be improved by providing more information regarding the number of films each year as well as analysis of the number of genre in one movie which might provide additional information about movies that have multiple genres as the reason of the rising trend of movies popularities. 

For question no.2, the limitations located in the statistical method that the researcher might have missed some of the proper procedures since the researcher only test and fix the linearity and multicollinearity while the normality and others violation might still being violated; however, the normality assumption violation might be okay to not be fixed as central limit theory stated that with high number of observations, the the error distribution are still often well-approximate near normal distribution.  
