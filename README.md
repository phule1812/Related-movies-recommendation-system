# Related movies recommendation
This project is a machine learning project that uses data about movies downloaded on the internet. Then, analyze that data and build a system to recommend similar movies according to the following criteria: relevance, genre and average rating of the given movie.

## Datasets : 
This Datasets for analysis and training are collected from MovieLens 20M Dataset in Kaggle. 

- Link to dataset : [http://grouplens.org/datasets/movielens/20m/](https://www.kaggle.com/datasets/grouplens/movielens-20m-dataset)

## Frameworks : 
* [Python](https://www.python.org/)
* [Numpy](https://numpy.org/)
* [Pandas](https://pandas.pydata.org/)
* [Scikit-learn](https://scikit-learn.org/stable/)

## Steps in the project : 
1. Analyze the dataset to find out the trends of movie genres.
2. Build a movie recommendation system based on K-Means.

## Result of project:
### 1. Analysis of the dataset 
From the collected data, two DataFrames representing information about movies and movie genres were found with the help of Pandas Framework.

* DataFrame representing information of movies was saved to the file 'movie_rating.csv'
* DataFrame representing information of movie genres was saved to the file 'Genre_Rating.csv'

Movies | Genres of movie 
:----|----:
![](image/movie_rating.png)|  ![](image/rating_by_genre.png)

From that, the trends of movie genres were found
Average rating of genres | Number of ratings of genres | Number movies of genres
:----|----|----:
![](image/ave_rating_of_genre.png) |  ![](image/num_of_ratings_of_genres.png)  | ![](image/number_movies_of_genres.png)

### 2. Model K-Means for recommendation of movies
* DataFrame for training model (df) was saved to file 'preparing_data_for_model.csv'

A model K-Means with 7 cluster was build to find related movies with given movie.

![](image/clusters.png)

When we give a my favourite movie, system will give us a list of 5 most similar movies, what we might be interested in:
![](image/recommend_movies.png)



