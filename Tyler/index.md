## Tyler's Page
Interest: I am interested in comparing the rating between recent release years for movies.

Data issues encountered: Our current dataset of netflix shows and movies currently contains a lot of information about the shows and movies on netflix however, it doesn't include the ratings the show/movies recieved. To attempt to gain access to the ratings I tried to use another dataset from IMDB and try and merge the data onto our current dataset to add ratings. However after furthur manipulation with the different datasets on IMDB I quickly came to the conclusion that the datasets were not only very impractical to use but the data doesn't seem to be accurate. Another issue with our datasets is that many of the foreign titles in our datasets seem to have their titles mistaken and their titles were entered using the wrong syntax. Another problem I came across is that the movies and tv-shows overlap on a lot of the rating when they shouldn't be overlapping. I think this is due to netflix having innconsistent identification on what's a tv show and whats a movie. To avoid this I will probably on work with movie ratings because those seem to be more or less fine.

### Netflix visualization
{% include_relative Visualization/test.html %}
{% include_relative Visualization/tvshows.html %}
{% include_relative Visualization/movies.html %}

### Comparing recent years rating distributions.
I am looking to compare the ratings distributions of movies based on release year and I will be specficially looking to focus on recent years. To do this I first looked to create a pie chart based on the rating of every movie in the dataframe so that we could compare each of the individual years to a baseline chart. After that I looked to create a pie chart for the ratings of the years 2020, 2019, 2018, 2017, 2016 and 2015.

### Baseline 
{% include_relative Visualization/movieratings.html %}
### 2020
{% include_relative Visualization/2020movies.html %}
### 2019
{% include_relative Visualization/2019movies.html %}
### 2018
{% include_relative Visualization/2018movies.html %}
### 2017
{% include_relative Visualization/2017movies.html %}
### 2016
{% include_relative Visualization/2016movies.html %}
### 2015
{% include_relative Visualization/2015movies.html %}


