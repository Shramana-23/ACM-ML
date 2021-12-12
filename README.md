RECOMMENDER SYSTEM OF ANIME DATASET USING COLLABORATIVE FILTERING

The dataset was taken from Kaggle
INFERENCE FROM THE DATASET-
1. Grouping the data by name and rating, the best rated movies are not the ones which have maximum number user ratings. So presumably the cause is rare movies have been rated
    the best by only a certain group of users who prefer those not by popularity but by their own choice.
2. Analysis into this shows that except for the movie 'Death Note', most of top movies also fall into the category of top genre
3. From the histogram of the number of ratings considering aggregation levels of genre and name of movies, we conclude that the maximum number of ratings fall in the bin size 
   of 0-1000 for both 'name' and 'genre'.

RECOMMENDER MODEL
1. The function get_recommendation is created based on user ratings and genre. At first, a list of animes with the same genre is created. Then we create a matrix based on the 
   generated list. Then we create a correlation matrix.
2. Finally calling get_recommendation function on a certain movie, we get a list with correlation and ratings sorted in decreasing order.
